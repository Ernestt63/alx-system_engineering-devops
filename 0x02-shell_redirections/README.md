A description of what the following scripts does in this directory.
echo "Hello, World" prints "Hello World"

echo "\"(Ôo)'" is used to write a script that displays a confused smiley "(Ôo)'.

cat /etc/passwd is used to display the content of the /etc/passwd file.

cat /etc/passwd  /etc/hosts is used to display the content of /etc/passwd and /etc/hosts

tail  /etc/passwd is used to display the last 10 lines of /etc/passwd

head -10 /etc/passwd is used to display the first 10 lines of /etc/passwd

head --lines=3 iacta | tail --lines=1 is used to write a script that displays the third line of the file iacta.

echo "Best School" > \\\*\\\\\'\"Best\ School\"\\\'\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\) is used to write a shell script that creates a file.

ls -la >> ls_cwd_content is used to write  a script that writes into the file ls_cwd_content

tail --lines=1 iacta >> iacta is used to write a script that duplicates the last line of the file iacta

find . -type f -name '*.js' -delete is used to write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.

find . -type d -path './*' -print | wc -l is used to write a script that counts the number of directories and sub-directories in the current directory.

ls -t | head is used to create  a script that displays the 10 newest files in the current directory.

sort | uniq -u is used to create a script that takes a list of words as input and prints only words that appear exactly once.

grep -i "root" /etc/passwd is used to display lines containing the pattern “root” from the file /etc/passwd

grep -c "bin" /etc/passwd is used to display the number of lines that contain the pattern “bin” in the file /etc/passwd

grep -iA 3 "root" /etc/passwd is used to display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.

grep -v "bin" /etc/passwd is used to display all the lines in the file /etc/passwd that do not contain the pattern “bin”.

grep '^[A-Za-z]' /etc/ssh/sshd_config is used to display all lines of the file /etc/ssh/sshd_config starting with a letter.

tr Ac Ze is used to replace all characters A and c from input to Z and e respectively.

tr -d cC is used to create a script that removes all letters c and C from input.

rev is used to write a script that revers
e its input.

cut -d':' -f1,6 /etc/passwd | sort is used to display all users and their home di
rectories, sorted by users.

find . -empty -printf %f'\n' is used to find all empty files and directories in the current directory and all sub-directories. 

find . -type f -name \*.gif -printf "%f\n" | LC_ALL=C sort -f | rev | cut -b 5- | rev is used to write a scrpt that lists all the files with a .gif extension in the current directory and all its sub-directories.

cut -c 1 | paste -s -d '' is used to create a script that decodes acrostics that use the first letter of each line.

tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev is used to write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
