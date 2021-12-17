

**LECTURE 6**

**VIM**

• Open vim > insert mode to write (i) > save ( Esc + : + w + filename+ enter) > save and quit ( esc +

: + w + q) > overwrite and save ( esc + : + q + !)

• To set line number: in commant mode: :set number

• No number: :set nonumber





**TAR command:**

• **TAR command is used to create and extract archive.**

• **To create: tar + options + archive name + files to add to archive (tar + filename.tar +**

• **To extract: tar + options + file to extract**





• **To create an archive: tar -cf example.tar file1 file2 file3**

• **-f is always required**

• **\* -v display the details. Not required**

• **To list the files in archive: tar tf filename.tar**

• **To add new file to the archive: tar rf filename.tar newfile.txt**

• **To update an existed file after edit: tar uf filename.tar newfile.txt**

• **To delete: tar --delete -f filename.tar filename.txt**

• **To move files to a new directory: tar -xf filename.tar -C newDir/**

• **To display all files including number in name for image and videos: tar cf allfiles.tar \*.txt \*[0-**

**9]\*.{jpg,png,svg} Video.mp4**

• **To generate a text file and save the output: lorem > filename.txt**





**CPIO**

• **CPIO is used to extract an archive**

• **To create an archive: ls | cpio -ov > nature.cpio**

• **To extract:**

**Ar**

• **To create an archive: ar r archive.a \***

• **List of the files: ar t archive.a**

• **To add new file: ar r archive.a newfile.txt**

• **To delete a file: ar d archice.a newfile.txt**

**Gzip**

• **Gzip filename.txt**

• **Compress multiple files: gzip file1.txt file2.txt file3.txt**

• **Compress and keep the original: gzip -k file.txt**

• **Decompress: gzip -d filename.txt**

• **Decompress a file from another directory to the present working directory: gzip -dkc <**

**../otherDirectoryName/filename.txt.gz > presentFile.txt**

File Permission:

\* To execute a file: chmod u+x filename.sh

\* To run the script: ./scriptname.sh

Symbolic mode

• u = user/owner, g = group, o = other

• r = read, w = write, x = execute

• To read, write, and execute: chmod u=rwx,g=rw,o=r

• Example: chmod u=rwe,g=rw,u=r filename.txt (user= rwe, group= rw, other = r)

Numeric mode

• Read = 4

• Write = 2

• Execute = 1

• RWe = 7, rw = 6, rx = 5

• Example: chmod 765 filename.txt (user= rwe, group= rw, other = r)


