```bash
sudo apt update

sudo apt install apache2 -y
```
List the `ufw` application profiles by typing:

```
sudo ufw app list
```

Copy

You will receive a list of the application profiles:

```
OutputAvailable applications:
  Apache
  Apache Full
  Apache Secure
  OpenSSH
```

As indicated by the output, there are three profiles available for Apache:

- **Apache**: This profile opens only port 80 (normal, unencrypted web traffic)
- **Apache Full**: This profile opens both port 80 (normal, unencrypted web traffic) and port 443 (TLS/SSL encrypted traffic)
- **Apache Secure**: This profile opens only port 443 (TLS/SSL encrypted traffic)

It is recommended that you enable the most restrictive profile that will still allow the traffic you’ve configured. Since we haven’t configured SSL for our server yet in this guide, we will only need to allow traffic on port 80:

```
sudo ufw allow 'Apache'
```

Copy

You can verify the change by typing:

```
sudo ufw status
```

Copy

The output will provide a list of allowed HTTP traffic:

```
OutputStatus: active

To                         Action      From
--                         ------      ----
OpenSSH                    ALLOW       Anywhere                  
Apache                     ALLOW       Anywhere                
OpenSSH (v6)               ALLOW       Anywhere (v6)             
Apache (v6)                ALLOW       Anywhere (v6)
```

As indicated by the output, the profile has been activated to allow access to the Apache web server.


Try typing this at your server’s command prompt:

```
hostname -I
```

Copy

You will get back a few addresses separated by spaces. You can try each in your web browser to determine if they work.

Another option is to use the Icanhazip tool, which should give you your public IP address as read from another location on the internet:

```
curl -4 icanhazip.com
```

When you have your server’s IP address, enter it into your browser’s address bar:

```
http://your_server_ip
```