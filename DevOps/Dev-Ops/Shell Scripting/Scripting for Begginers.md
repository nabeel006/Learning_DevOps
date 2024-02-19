


The back-ticks used for command substitution like a command within the command
Alternatively, you can also use the modern syntax `$()` for command substitution instead of back-ticks:

```bash
echo "Today is " `date`
myvar="Hello";

echo "Nabeel 

And now use it with Veriables

$myvar"


[fchen14@mike1 ~]$ str1='echo $USER' 
[fchen14@mike1 ~]$ echo "$str1" 
echo $USER 
[fchen14@mike1 ~]$ str2="echo $USER" 
[fchen14@mike1 ~]$ echo "$str2" 
echo fchen14 
[fchen14@mike1 ~]$ str3=`echo $USER` 
[fchen14@mike1 ~]$ echo $str3 
fchen14 
[fchen14@mike1 ~]$ str3=$(echo $USER)
fchen14
[fchen14@mike1 ~]$ echo "$str3" 
fchen14

```


### Reading from a file
```bash
while read line
do
  echo $line
done < input.txt
```