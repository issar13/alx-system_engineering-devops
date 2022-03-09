## Shell Redirections Project Tasks

**Task 0:** **echo Hello, World:** Print Hello, World.

**Task 1:** **echo "\"(Ôo)'":** Print the smiley confused emote.

**Task 2:** **cat /etc/passwd:** Displays contents of etc/password using cat.

**Task 3:** **cat /etc/password /etc/hosts:** Displays contents of etc/passwords||etc/hosts

**Task 4:** **tail /etc/passwd:** Displays the last 10 lines of /etc/passwd

**Task 5:** **head /etc/passwd:** Displays the first 10 lines of etc/password

**Task 6:** **head --lines=3 iacta | tail --lines=1:**  Script that displays the third line of the file iacta.

**Task 7:** **echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)":** create a file with many slashes, thats' it.

**Task 8:** **ls -la > ls_cwd_content:** write into ls_cwd_content the result of the command ls -la.

**Task 9:** **echo -en "" | tail --lines=1 iacta >> iacta:** Write a script that duplicates the last line of the file iacta

**Task 10:** **find . -name '*.js' -type f -delete:** find .js files in folders and directories and delete.

**Task 11:** **find -mindepth 1 -type d | wc -l.:** script that counts the number of directories and sub-directories in the current directory.

**Task 12:** **ls -t | head:** Script that displays the 10 newest files in the current directory.

**Task 13:** **sort | uniq -u:** a script that takes a list of words as input and prints only words that appear exactly once.

**Task 14:** **grep -i root /etc/passwd:** script that displays the lines containing the pattern “root” from the file /etc/passwd

**Task 15:** **grep -i bin /etc/passwd | wc -l:** script that displays lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.

**Task 16:** **grep -iA 3 root /etc/passwd:** Displays lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.

**Task 17:** **grep -iv bin /etc/passwd:** Displays all the lines in the file /etc/passwd that do not contain the pattern “bin”.

**Task 18:** **grep -i "^[a-z]" /etc/ssh/sshd_config:** Display all lines of the file /etc/ssh/sshd_config starting with a letter.

**Task 19:** **tr Ac Ze:** Script that replaces all characters A and c from input to Z and e respectively.

**Task 20:** **tr -d cC:** creates a script that removes all letters c and C from input.

**Task 21:** **rev:** script that reverses it's input.

**Task 22:** **cut -d':' -f1,6 /etc/passwd | sort:** Writes a script that displays all users and their home directories, sorted by users.

**Task 23:** **find . -empty -printf "%f\n":** Script that finds all empty files and directories in the current directory and all sub-directories. only the names of the files and directories should be displayed,Hidden files should be listed,One file name per line and 
the listing should end with a new line

**Task 24:** **find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f:** Write a script that lists all the files with a .gif extension in the current directory and all its sub-directories,hidden files should be listed,only regular files (not directories) should be listed,the names of the files should be displayed without their extension,the files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay),One file name per line,The listing should end with a new line

**Task 25:** **cut -c 1 | tr -d '\n' | sort:** Create a script that decodes acrostics that use the first letter of each line.The ‘decoded’ message has to end with a new line.

**Task 26:** **tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev:** Write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests. Order by number of requests, most active host or IP at the top.



