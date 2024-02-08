**
```bash
How to show only a given line or range of lines?


sed -n '1p' file_name

sed -n '1,5p' file_name

sed -n '$p' file_name


  

How to see all the users from India Country?

sed -n '/India/p' file_name

  
  

How to use multiple expression in sed command?

Example: If you wanna only see 2 and 5th line

sed -n -e '2p' -e '5p' file_name

  

How to see all the users from India and Germany?

sed -n -e '/India/p' -e '/Germany/p' file_name

  
  

How to see next 4 lines from 2nd line?

sed -n ‘2,+4p’ file_name

  

How to see every 2nd line from first line?

sed -n ‘1~2p’ file_name

  

How to read expression from external file?

sed -f ex_file file_name

  

How to replace a word in a file and show?

sed 's/<string_to_change>/<new_string>/g' file_name

  

How to replace a word in a file and show except a given line or only in given line?

sed '5 s/<string_to_change>/<new_string>/g' file_name

sed '5! s/<string_to_change>/<new_string>/g' file_name

  

How to replace a word and and edit in your file?

sed -i's/<string_to_change>/<new_string>/g' file_name

  

How to change salary or country of a user (Paul)?

sed '/Paul/ s/25000/35000/g' file_name

sed '/Paul/ s/India/US/g' file_name

  
  

How to delete a line?

sed '1d' file_name                                    (to delete first line)

sed '1,2d' file_name

sed '$d' file_name

  

How to delete user from India country?

sed ‘/India/d’ file_name
```

