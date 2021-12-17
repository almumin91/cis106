

**Lecture 7**

**Managing user accounts**

• **It involves adding, modifying and deleting user accounts and information.**

• **To add user acc: user add or adduser (user add is low level utility, later one is better**

**command)**

o **Example: sudo adduser abd007 (then create a password)**

• **To modify user info: usermod**

• **To delete: userdel**

o **Example: sudo userdel -r abd007**

• **Following files are involved in the user creation process:**

o **/etc/login.defs**

o **/etc/default/useradd**

o **/etc/skel/**

o **/etc/passwd**

o **/etc/shadow**

o **/etc/group**

• **/etc/login.defs file: grep -ve ^$ /etc/login.defs | grep -v ^#**

o **First grep command will suppress all empty lines, second grep will suppress all**

**comments which are lines that start with the # symbol**

• **To view the default parameters in the /etc/defau;t/useradd file: useradd -d or cat**

**/etc/default/useradd**

• **The /etc/passwd file stores information about every avvount in a linux system.**

• **Each line = a user**

• **Entries in the passwd file contains I fields divided by a:**

• **To see students user info: grep student /etc/passwd**

**To view info about user’s acc n passwd: getent passwd student, sudo getent shadow student**

• **To update passwd for current user: sudo passwd**

• **To update psaswd for another user: sudo passwd + username**

• **To lock and unlock account: suto passwd -l or pass -u**

• **Create a home directory for user: sudo usermod -md /home/abd007 abd007**

• **Loging with new user : su username**

• **Logit: exit**

• **Change the default shell: sudo usermod -s /bin/bash username**

**Managing Group:**

• **Cat /etc/passwd | grep “Adrian”**

• **Cat /etc/passwd | ^”Adrian”**

• **Sudo groups Adrian**


