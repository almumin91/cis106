

**LECTURE 5**

**Handling Text File**

**Cat**

• The Cat command is used for displaying the content of a file.

• Cat is short of concatenate which is the command intended use.

• It means joining two strings together.

• Example: cat todo.md

**Tac**

• Tac displays the files from tail to head (reverse order).

• It can also concatenate two files

**More**

• The more command is a pager program used for displaying the content of a text file one

page at a time.

• Ex: more + file to view

• To display first 10 lines of a file: head /etc/passwd

• To display first 5 lines of a file: head -5 /etc/passwd

• **To Display last 5 lines: tail -5 /etc/passwd**

**Cut**

• Allows you to extract files from a specific field

• Display the last 5 users: tail -5 /etc/passwd | cut -d ‘:’ -f 1

**Sort**

• Sort -o filename.txt oldname.txt (to sort the file and save with a new name)

• Sort with numeric data: sort -n filename.txt

• Check if a file is sorted: sort -c filename

• Sort in reverse order: sort -r filename

• Sort by column number: sort -k 2 fileName

• Remove duplicate user: sort -u filename

**Grep**

• The **Grep** command is used to match a string pattern from a file.

• Example: grep + option + Pattern to match + file





•

Match all lines that start with uppercase letters

grep "^[[:upper:]]" /etc/passwd

Match all lines that end with a digit

grep "[[:digit:]]$ data.csv"

Match only lines containing IPv4 addresses

grep -E

'[[:digit:]]{1,3}\.[[:digit:]]{1,3}\.[[:digit:]]{1,3}\

.[[:digit:]]{1,3}' ipaddresses

Match one word or the other.

grep -E 'hello|hi' file.txt

Grep can search for pattern sequences using {n}

Search all lines that contain a character repeated 3 times

grep -E "A{3}" file.txt

Search all lines that contain a phone number of the format 973-111-2222

grep "[[:digit:]]\{3\}[-][[:digit:]]\{3\}[-

][[:digit:]]\{4\}" file

The period character (.) is used to represent any single character. For example, search

for all lines that contain any word ending in "able" and has 3 characters before "able".

grep "...able" logbackup.log

• abd007@cis240-fall21:~$ man ls | grep "comma separated"

• output:

-m fill width with a comma separated list of entries

•

**I/O (input/output) Redirection**

