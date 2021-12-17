

**Lecture 4**

\- cd/ will takes to root

\- shortcuts of cd

\- cd/usr/share/theme – absolute path (starts on the root)

\- ls to see the lists

\- cd Music / (relative path to home directory)

\- mkdir is to make dir

\- mkdir ~/drinks is an easy way to create a dir

\- String: holds a data type.

\- Mkdir (-p) will be in mids meaning parent folder.

\- To create a file: touch filename

\-





**INODES (index files)**

• A data structure that contains all the information about a file except the file name and

its content.

• Every file in the file system has an inode

• To know the the created file location: ls -I ~/filename.

**Hard Links**

• To create a hard link: ln file ~/Downloads/FileHL

o abd007@cis240-fall21:~$ ln file1 Downloads/file1-hl

o abd007@cis240-fall21:~$ ls -i file1 Downloads/file1-hl -1

o 656004 Downloads/file1-hl

o 656004 file1

o abd007@cis240-fall21:~$

• The hard link needs to be the same file system to create links between them. ( ext – ext=

link; fat32 -ext= no link)

• It’s the direct connection to the file





**Soft Links**

• Soft connection between files.

• Connect to the hard link and not directly to the data/file.

• To create a symbolic link: ln -s fileName fileNameSL

• The advantage of soft li’nks is that they can point to files that are stored in different

positions

o **abd007@cis240-fall21:~$ ln -s file1 softhere**

o **abd007@cis240-fall21:~$ stat file1**

o **File: file1**

o **Size: 0**

**Blocks: 0**

**IO Block: 4096 regular empty file**

o **Device: 805h/2053d Inode: 656004 Links: 3**

o **Access: (0664/-rw-rw-r--) Uid: ( 1000/ abd007) Gid: ( 1000/ abd007)**

o **Access: 2021-10-20 17:50:16.249998976 -0400**

o **Modify: 2021-10-20 17:50:16.249998976 -0400**

o **Change: 2021-10-20 18:01:29.494487106 -0400**

o **Birth: -**

o **abd007@cis240-fall21:~$ ls -l softhere**

o **lrwxrwxrwx 1 abd007 abd007 5 Oct 20 18:14 softhere -> file1**

o **abd007@cis240-fall21:~$**

### Using wildcards/ File globbing

• Wildcard represents letters and characters used to specify a filename for searches

• File globbing is the processing of pattern matching using wildcards.\

• The wildcards are officially called metacharacter wildcards





**The \* wildcard:**

**The ? wildcard**

• The ‘?’ wildcard meta character matches precisely one character. You might need the

question mark to minimize a long list of files names down to a few.

**The [] character**

• The brackets wildcard match a single character in a range.

