Introduction to Linux – Full Course for Beginners

https://www.youtube.com/watch?v=sWbUDq4S6Y8 

https://www.linuxfoundation.org/ 

Chapter 1
Introduction to Linux Families

Describe software required
Describe the major Linux distro families

Course Requirements 

Red Hat Family System ( CentOS and Fedora )
SUSE Family Systems ( Open SUSE )
Debian Family Systems ( Ubuntu and Linux Mint )

                                                  Linux Kernel
Distro Families    Debian           RHEL                         SUSE        Other Distributions 

                            Ubuntu               Fedora                   SLES
Individual             Linux Mint                                         open SUSE
Distros                                  CentOS  Oracle Linux

Red Hat Family
Red Hat Enterprise Linux
CentOS
CentOS Stream
Fedora
Oracle Linux

Key Facts About the Red Hat Family
Fedora an upstream testing platform
CentOS is a close clone of RHEL
Intel x86, Arm, Itanium, PowerPC
yum package manager
Widely used by enterprises

The SUSE Family
Key Facts About the SUSE Family
SUSE Linux Enterprise Server (SLES) is upstream for openSUSE
RPM-based zypper package manager 
YaST for system admin purposes 
Widely used in retail 

The Debian Family
Ubuntu 
Ubuntu Mint

Ubuntu (LTS) - Long Term Support
Key Facts About the Debian Family
Debian family is upstream for Ubuntu
DPKG-based APT package manager
Widely used for cloud deployments
GNOME-based but differs visually 

Chapter 2 
Linux Philosophy and Concepts 
Define common Linux terms
Discuss components of Linux distro

Linux Terminology and Examples
Kernel: Glue between hardware and applications. Ex: Linux Kernel 

Distribution
Boot Loader: Program that boots the operating system. Ex: GRUB and ISOLINUX

Service: Program that runs as a background process. Ex: httpd, nfsd, ntpd, ftpd and named

Filesystem: Method for storing and organizing files. Ex: ext3, ext4, FAT, XFS, NTFS and Btrfs

X Window System: Graphical subsystem on nearly all Linux Systems
GUI
Desktop
(KDE, GNOME.XFCE)
Window 
Manager
X Window System
X11
Console
CLI/Shell
KERNEL
Hardware

Desktop Environment: Graphical user interface on top of the operating system. Ex: GNOME, KDE, Xfce and Fluxbox

Command Line: Interface for typing commands on top of the operating system

Shell: Command line interpreter that interprets the command line input and instructs the operating system to perform any necessary tasks and commands. Ex: bash, tcsh, zsh

Linux Distributions 
Applications
Kernel
CPU Memory Devices

https://www.kernel.org/ 

Linux Kernel
Documentation for: Commands, Applications, Services
Libraries, Utilities, Configuration
Applications
Package Updates, Upgrades, Kernel and Driver patches
Support Services: Commercial, Community

Services Associated with Distributions
Linux Support and Services 
Community Support and Services
CentOS
openSUSE
Ubuntu Community Support
Commercial Support and Services
Oracle
RHEL
SLES
Ubuntu Commercial Support

Linux borrows from UNIX
Linux accesses features through files
Linux is a multi tasking OS
Terms: Kernel, Distribution, Boot Loader
Linux distro includes kernel and tools

Chapter 3
Linux Basics and System Startup 

Identify Linux File Systems
Identify differences: partitions vs filesystem
Describe the boot process 
Install linux on a computer 

Power On

BIOS
BIOS: The First Step
Power On
BIOS ( Basic Input/Output System )
Initialize the screen and keyboard and test the main memory

Master Boot Record ( MRB ) also known as First Sector of the Hard Disk
Master Boot Record ( MBR ) and Boot Loader
Master Boot Record ( MBR )
Partition 1            Partition 2              Partition 3
( Bootable ) 
Searches for GRUB and loads it into RAM

Boot Loader ( e.g.GRUB ) - Responsible for load the kernel image and initial Ram disk or file System into memory
GNU GRUB version 1.97~beta4
Ubuntu, Linux 2.6.31-14-generic 
…
Master Boot Record ( 512 bytes )
System
Bootable Hard Disk
Boot Loader
Kernel            Initial RAM Disk

Kernel ( Linux OS )

Initial Ram disk - initramfs image
initramfs
Programs 
Binary Files
Mount proper root filesystem
Providing kernel functionality 
Locating devices
Locating drivers and load them
Checking for errors in root filesystem
Text-Mode login 
Init 
Username
Password
Command Shell
ie.bash
( the GNU Bourne Again Shell )
The Linux Kernel 
Boot loader
Kernel          RAM-based filesystem
Memory

/sbin/init ( parent process )
Kernel
/sbin/init
Starts other process to get the system running 
Systemd
systemctl 
Linux Filesystem Basics
Conventional Disk Filesystems ( ext3, ext4, XFS, Btrfs, JFS, NTFS, vfat, etc )
Flash Storage Filesystems ( ubifs, jffs2, yaffs, etc )
Database Filesystems
Special Purpose Filesystems ( procfs, sysfs, tmpfs, aquashfs, debugfs, etc )
Partition and Filesystems
                                                Windows                               Linux 
Partition                                               Disk1                                    /dev/sda1
Filesystem Type                                   NTFS/VFAT                        EXT3, EXT4, XFS, BTRFS
Mounting Parameters                           DriverLetter                           MountPoint
Base Folder ( Where OS is stored )    C:\                                         /
The Filesystem Hierarchy Standard ( FHS )

Typical Ubuntu Filesystem Hierarchy 


 
Command Shell using getty
X Windows System ( Graphical User Interface ) 

Linux Distribution Installation 

Server
RHEL/CentOS
Ubuntu Server
SLES
Debian
Desktop
Ubuntu
Fedora
Linux Mint
Debian
Embedded
Yocto
Open Embedded
Android 

Linux Installation Planning 
Partitions in the Linux Hard Disk
/(sda1)                                            home(sda2)
                Linux Hard Disk (sda)
            var (sda3)                                       swap(sda4)
Linux Installation: Software Choices
Category 1:: Physical media: CD, DVD, USB, or HDD

Category 2:: Network media: HTTP, FTP, NFS

 

In addition, the installation methods can be categorizes into 4 major categories:

Method 1:: Clean: installation that does not write to current OS storage media

Method 2:: Dual-boot: peaceful co-existence with current OS on same storage media

Method 3:: Replacement: overwriting of current OS with Linux on platform storage media

Method 4:: Upgrading: enhancing current OS to newer or different version of Linux OS
Linux Installation: Install Source ( The Process ) 
https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview 

Chapter 4
Graphical Interface
Manage graphical interfaces
Perform operations with GUI
Change graphical desktop
Command Line Interface or Graphical User Interface
Rodrigo@ubuntu:~$ cd Documents 
Rodrigo@ubuntu:~/Documents$ touch hello.txt
Rodrigo@ubuntu:~/Documents$ nano hello.txt
hello

Red Hat
CentOs 
Fedora
SUSE 
Open SUSE
Debian 
Ubuntu
Ubuntu Mint

Desktop Environment 
Session Manager
Window Manager

Chapter 5
System Configuration from the Graphical Interface
Use the System Settings panel
Specifying Screen Resolution

Use the Network Manager
Managing network connections

Install and Update software
Changing the date and time 

System, Display, Date and Time Settings

System Settings Menus
Devices
Users
Login Picture
Password

Gnome-Tweaks
Alt-F2
Selecting a Theme
Configuring Extensions
Control Fonts
Modify Keyboard Layout
Set Programs

Display Settings 
Linux Distribution
Particular Version
Display Panel

X Server ( GUI )
/etc/X11/xorg.conf

Setting Resolution and Configuring Multiple Screens
Displays

Network Time Protocol
Network Configuration Files
Wired and Wireless Connections
Dynamic Host Configuration Protocol ( DHCP )
Media Access Control Address
Configuring Wireless Connections
Mobile Broadband and VPN Connections
Installing and Updating Software
Linux Kernel
C Compiler
Utilities ( High Level Utilitie ) 
Debian Packaging ( Debian Family System ) 
Debian Based Systems
Apt
dpkg-installer
Debian Family Linux
apt-get
Synaptic
Ubuntu Software Center

Red Hat Package Manager ( RPM )
SUSE/openSUSE
CentOS
Oracle Linux
Yum
RPM-Installer
Fedora Family Linux

OpenSUSE´s YaST Software Management 
Click Activities 
In the search box, type YaST
Click in the YaST Icon
Click Software Management
YaST Software Manager
RPM-Installer
SUSE Family Linux

Installing and Updating Software in openSUSE
Installing and Updating Software in Ubuntu

Chapter 6
Common Applications
Internet Applications
Web Browsers
Firefox
Chrome
Epiphany

Email Clients 
Thunderbird
Evolution
Mutt

Email Applications
Graphical ( Thunderbird, Evolution, Claws Mail )
Text ( Mutt, Mail ) 

Online Media Applications 
Amarok
Audacity
Rhythmbox

Productivity Applications
Other Applications 
Pidgin 
Filezilla
Xchat
Pidgin
Ekiga

Office Productivity Suites
Text
SpreadSheets
Presentations
Graphical Objects
LibreOffice ( Writer, Calc, Impress )

Developer Tool
Multimedia Applications
Audacity
Amarok
Movie Players 
VLC
Xine
MPlayer
Totem
Movie Editors
Cinepaint
Blender
Cinelerra
Ffmpeg

Graphics Editors
Gimp
Handle any file format
Special purpose plugins and filters
Extensive information about the image 
Inkscape
Eye of Gnome
Image Magick

Chapter 8
Command Line Operations 
Use the command line
Using a Text Terminal on the graphical desktop
admin@ubuntu:~$ useradd -m -c “alexis” -s/bin/bash alexis
useradd: Permission denied.
useradd: cannot lock /etc/passwd; try again later.
admin@ubuntu:~$
Launching Terminal Windows
Applications > Utilities > Terminal 
Basic Utilities
cat: used to type out a file ( or combine files )
head: used to show the first few lines of a file
tail: used to show the last few lines of a file
man: used to view documentation
command       -options       arguments
Is                    -a                  /home/angela

Steps for Setting UP and Running Sudo
sudo ( CLI pormpt “su” )
$ su Password:
# echo “student ALL=(ALL) ALL” > /etc/sudoers.d/student
# chmod 440 /ect/sudoers.d/student
etc/sudoerc.d/

student@openSUSE:~$ sudo ls -la / root
Switching Between the GUI and the Command Line
Virtual Terminals
Turning Off the Graphical Desktop
telinit
$ sudo systemctl stop gdm ( or sudo telinit 3 )
$ sudo systemctl start gdm ( or sudo telinit 5 )
substitute lightdm for gdm
Basic Operations 
cd
cat
echo
ls
rmdir
man
exit 
login
mkdir
Login in and Log Out
Rebooting and Shutting Down
halt
poweroff
shutdown -h
shutdown -r
Locating Applications
/bin
/usr/bin
/sbin
/usr/sbin
/opt
/usr/local/bin
/usr/local/sbin
/home/student/bin
$ which diff
/usr/bin/diff
Accessing Directories
$ echo $home
$HOME/Desktop
Command                                     Result
pwd                                Displays the present working directory
cd ~ or cd                       Change to your home directory ( shortcut name is ~( tilde ))
cd ..                                Change to parent directory 
cd -                                 Change to previous directory ( - ( minus ))

[student@c8stream usr]$ cd /tmp
[student@c8stream tmp]$ pwd
/tmp
[student@c8stream tmp]$ cd $HOME
[student@c8stream tmp]$ pwd
/home/student
[student@c8stream ~]$cd ..
[student@c8stream home]$ pwd
/home
[student@c8stream home]$ pushd /tmp
/tmp /home
[student@c8stream tmp]$ popd
/home
[student@c8stream home]$ cd -
/tmp
[student@c8stream tmp]$ 

Understanding Absolute and Relative Paths

. ( present directory )
.. ( parent directory )
~ (your home directory )
Absolute pathname method
$ cd/usr/bin
Relative pathname method
$ cd../../usr/bin

Exploring the file System
Command                             Usage
cd /                     Changes your current directory to the root(/) directory ( or path you supply )
ls                         List the contents of the present working directory
ls -a                     List all files, including hidden files and directories ( name start with . )
tree                     Display a tree view of the filesystem 

Search for files
test1@ubuntu:/$ cd usr/local/lib
test1@ubuntu:/usr/local/lib$ cd /usr
test1@ubuntu:/usr$ cd loca/lib
test1@ubuntu:/usr/local/lib$ cd /
test1@ubuntu:/$ ls
bin     cdrom etc       initrd.img   lib64            media  nfs   proc   run    srv   tmp var
boot   dev     home   lib              lost+found   mnt     opt    root   sbin   sys  usr  vmlinuz
test1@ubuntu:/$ ls -a
. bin     cdrom etc       initrd.img   lib64            media  nfs   proc   run    srv   tmp var
.. boot   dev     home   lib              lost+found   mnt     opt    root   sbin   sys  usr  vmlinuz
test1@ubuntu:/$ tree
test1@ubuntu:/$ tree -d /

Hard Links
$ Ln file1 file2
$ Ln -li file1 file2

soft ( symbolic ) Links
$ Ls -s file1 file3
$ Ls -li file1 file3

Navigating the Directory History
$ cd -
[student@fedora ~]$ mkdir /tmp/dir1 /tmp/dir2
[student@fedora ~]$ pushd /tmp/dir1
/tmp/dir1 ~
[student@fedora dir1]$ pushd /tmp/dir2
/tmp/dir2 /tmp/dir1 ~
[student@fedora dir2]$ popd 
/tmp/dir1 
[student@fedora dir1]$ popd
~
[student@fedora ~]$  

Create and manage files
Working with Files 
[student@c8stream LFT]$ wc ready-for.sh
 5127 16626 198629 ready-for.sh
[student@c8stream LFT]$ cat ready-for.sh
[student@c8stream LFT]$ cat -n ready-for.sh
[student@c8stream LFT]$ less ready-for.sh
[student@c8stream LFT]$ less -N ready-for.sh
[student@c8stream LFT]$ head ready-for.sh
[student@c8stream LFT]$ head -20 ready-for.sh
[student@c8stream LFT]$ tail ready-for.sh
[student@c8stream LFT]$ tail -20 ready-for.sh
[student@c8stream LFT]$ tac ready-for.sh

touch 
$ touch <filename>

mkdir and rmdir
$ mkdir sampdir
$ mkdir /usr/sampdir
$ rm -rf

Moving, Renaming or Removing a File
Command                             Usage
mv                                      Rename a file
rm                                       Remove a file
rm -f                                    Forcefully remove a file
rm -i                                    Interactively remove a file

Rename or Removing a Directory
Command                              Usage
mv                                       Rename a directory
rmdir                                    Remove an empty directory
rm -rf                                   Forcefully remove a directory recursively 

Modifying the Command Line Prompt
student@c8 $
\u@\h\$
$ echo $SP1
\$
$ PS1=“u@\h \$”
student@c8 $ echo $ SP1
\u@\h \$
student@c8 $
 
[student@c8stream tmp]$ echo > file1
[student@c8stream tmp]$ touch file2
[student@c8stream tmp]$ ls -l file1 file2 
-rm-rw-r- - 1 student student 1 Jul 14 16:31 file1
-rm-rw-r- - 1 student student 0 Jul 14 16:31 file2
[student@c8stream tmp]$ mv file1 file1-newname
[student@c8stream tmp]$ ls -l *file*
-rm-rw-r- - 1 student student 1 Jul 14 16:31 file1-newname
-rm-rw-r- - 1 student student 0 Jul 14 16:31 file2
[student@c8stream tmp]$ rm file2
[student@c8stream tmp]$ rm -i file1-newname
rm: remove regular file ‘file1-newname’? y
[student@c8stream tmp]$ mkdir dir1
[student@c8stream tmp]$ mkdir dir2 dir3
[student@c8stream tmp]$ ls -l
total 12
drwxrwxr-x 2 student student 4096 Jul 14 16:33 dir1
drwxrwxr-x 2 student student 4096 Jul 14 16:33 dir2
drwxrwxr-x 2 student student 4096 Jul 14 16:33 dir3
[student@c8stream tmp]$ touch dir2/file1
[student@c8stream tmp]$ touch dir2/file2
[student@c8stream tmp]$ ls -lR dir*
dir1:
total 0

dir2:
-rm-rw-r- - 1 student student 1 Jul 14 16:33 file1
-rm-rw-r- - 1 student student 1 Jul 14 16:33 file2

dir3:
total 0
[student@c8stream tmp]$ rmdir dir*
rmdir: failed to remove ‘dir2’: Directory not empty
[student@c8stream tmp]$ ls -l
total 4
drwxrwxr-x 2 student student 4096 Jul 14 16:33 dir2
[student@c8stream tmp]$ rm -rf dir2
[student@c8stream tmp]$ 

Standart Files Streams
Name                  Symbolic Name       Value       Example
standart input      stdin                         0              keyboard
standart output    stout                         1              terminal 
standart error      stderr                        2              log file

I/O Redirection
$ do_something < input-file
$ do_something > output-file
$ do_something 2> error-file
$ do_something > all-output-file 2>&1
$ do_something >& all-output-file

Pipes
$ command1 | command2 | command3 
Process1   | ->  Process2   | ->   Process3  | ->   Process4     
               Pipe1                 Pipe2                Pipe3

Searching for Files

Locate
grep
$ locate zip | grep bin

student@ubuntu:~$ locate LFS300
/home/student/LFT/LFS300_VS.0_SOLUTIONS.tar.xz
student@ubuntu:~$ find .name “LFS300*”
./LFT/LFS300_VS.0_SOLUTIONS.tar.xz
student@ubuntu:~$  find .name “LFS300*” -ls
 1721851        4  -rw-rw-r- -  1  student  student   3592  feb  2   12:30    ./LFT/LF  
S300_VS.0_SOLUTIONS.tar.xz
student@ubuntu:~$ echo > LFS300
student@ubuntu:~$ find . -name “LFS300*” -ls
1721851         4 -rw-rw-r- -    1 student   student    3592 Feb  2   12:30   ./LFT/LF
S300_V5.0_SOLUTIONS.tar.xz
1704052         4 -rw-rw-r- -     1 student  student    1       Jul   7    10:20    ./LFS300
student@ubuntu:~$ locate LFS300
/home/student/LFT/LFS300_v5.0_SOLUTIONS.tar.xz
student@ubuntu:~$ sudo updatedb
student@ubuntu:~$ locate LFS300
/home/student/LFS300
/home/student/LFT/LFS300_v5.0_SOLUTIONS.tar.xz
student@ubuntu:~$ rm LFS300
student@ubuntu:~$ updatedb
updatedb: can not open temporary file for ´/var/lib/mlocate/mlocate.db’
student@ubuntu:~$ sudo updatedb
student@ubuntu:~$ locate LFS300
/home/student/LFT/LFS300_v5.0_SOLUTIONS.tar.xz
student@ubuntu:~$ cd /etc/
student@ubuntu:/etc$ cat updatedb.conf
PRUNE_BIND_MOUNTS=“yes”
# PRUNENAMES=“.git .bzr .hg .svn”
PRUNEPATHS=“...
…
student@ubuntu:/etc$ 

Wildcards and Matching File Names
Wildcard       Result
?                   Matches any single character 
*        Matches any string of character
[set]              Matches any character in the set of characters, Ex: [adf] will match any occurrence of a, d or f
[!set]            Matches any character not in the set of character

$ ls * .out

student@ubuntu:/var/log$ ls
alternatives.log     auth.log.1     dmesg   fontconfig.log  kern.log2.gz   speech-dispatcher …
…
student@ubuntu:/var/log$ du -sh a*
0         alternatives.log
4.0K    alternatives.log.1
4.0K    alternatives.log.2.gz
0         apport.log 
…
student@ubuntu:/var/log$ du -sh *alog*
0         alternatives.log
4.0K    alternatives.log.1
4.0K    alternatives.log.2.gz
0         apport.log 
student@ubuntu:/var/log$ du -sh a[p-z]*
0         apport.log 
4.0K    alternatives.log.1
4.0K    alternatives.log.2.gz
248K   apt
…
student@ubuntu:/var/log$ du *.?.*
4        alternatives.log.2.gz
4        apport.log.2.gz
8        auth.log.2.gz
4        btmp.1.gz
…
student@ubuntu:/var/log$ sudo apt-get install vmware*
…
student@ubuntu:/var/log$ sudo apt-get install “vmware*”
student@ubuntu:/var/log$ 

Install and update software

The Find Program

student@ubuntu:/var/log$ sudo find . -name “*.log”

Using Find
-name 
-iname
-type
d - directory 
L - symbolic link
f - regular file - c7:/tmp>  sudo find -type f -name gcc

c7:/tmp> sudo find /usr -name gcc

Using Advanced Find Options 
-exec
$ find -name “*.swp” -exec rm { } ‘;’
‘;’
“\;” 

$ find -name “*.swap” -exec rm { } ‘;’
Finds and Removes files that ends with .swp
*.swp

Find Files Based on Time and Size
$ find / -ctime 3
-cmin, -amin, and -mmin
$ find / -size 0

c7:/usr/src>find lin* -size +10M -exec ls -shF { } ‘;’ 

student@ubuntu:/var/log$ sudo find .
./kern.log
./bootstrap.log
./mail.log
./btmp.1.gz
…
student@ubuntu:/var/log$ sudo find . -type d
.
./gdm3
./libvirt
./libvirt.uml
…
student@ubuntu:/var/log$ find . -type f -exec grep -H log {} \; 
…
student@ubuntu:/var/log$ find . -type f -exec ls -l {} \;
…
student@ubuntu:/var/log$ find -type f -ls
…
student@ubuntu:/var/log$ find . -size 0
find: ‘./gdm3’ : permission denied
…
student@ubuntu:/var/log$ sudo find . -size 0
./libvirt/uml/.placeholder
…
student@ubuntu:/var/log$ sudo find . -size 0 -ls 
…
student@ubuntu:/var/log$ sudo find . -newer btmp
…
student@ubuntu:/var/log$ 

Packages Management Systems on Linux

Package Manager: Two Levels
Linux 
Package Manager  Debian Family System   SUSE Family System   Red hat Family System
High Level
Package Manager  apt-get                            zypper                           yum
Low Level
Package Manager  dpkg                                                     rpm
                                               Linux System

Working with Different Package Management Systems
Linux 
Package Manager  Debian Family System   SUSE Family System   Red hat Family System
High Level
Package Manager  apt-get                            zypper                           yum

dnf ( Open Source Command Line Package Management Utility )
rpm ( Head Hat Family System ) 
CLI and GUI 

Operation                                          rpm                                             deb
Install package                                  rpm -i foo .rpm                            dpkg - -install foo.deb      
Install package, dependencies         dnf install foo                               apt-get install foo
Remove package                              rpm -e foo .rpm                           dpkg - -remove foo.deb
Remove package, dependencies     dnf remove foo                            apt-get autoremove foo
Update package                                rpm -U foo.rpm                            dpkg - -install foo.deb
Update package, dependencies       dnf update foo                             apr-get install foo
Update entire system                        dnf update                                   apt-get dist-upgrade
Show all installed packages             rpm -qa or dnf list installed           dpkg - -list
Get information on package              rpm -qil foo                                  dpkg -listfiles foo
Show packages named foo               dnf list “foo”                                 apt-cache search foo
Show all available packages             dnf list                                       apt-cache dumpavail foo
What package is file part of ?            rpm -qf file                                   dpkg - -search file 

student@debian:~$ dpkg - -list | less
Desired=Unknown/Install/Remove/Purge/Hold
…
student@debian:~$ dpkg - -list
…
student@debian:~$ dpkg - -list | grep bzip2
ri bzip2                                                            1.0.6-8.1    amd64     
orting file compressor - utilities 
student@debian:~$ dpkg - -listfiles bzip2 | less
/.
/bin
/bin/bunzip2
/bin/bzcat
…
student@debian:~$ sudo dpkg - -remove bzip2 
…
student@debian:~$ 

[student@CentOS7 ~]$ rpm -qa | grep bzip2
bzip2-1.0.6-13.el7.x86_64
bzip2-list-1.0.6-13.el7.x86_64
[student@CentOS7 ~]$ rpm -qil bzip2 | less
Name           : bzip2
Version         : 1.0.6
Release       : 13.el7
Architecture : x86_64
…
[student@CentOS7 ~]$ ls -lF $(rom -ql bzip2) | less
…
[student@CentOS7 ~]$ sudo rpm -e - -test bzip2
…
[student@CentOS7 ~]$ rpm -q - -whatprovides bzip2
bzip2-1.0.6-13.el7.x86_64
[student@CentOS7 ~]$ rpm -q - -whatrequires bzip2
sos-3.3-5.el7.centos.noarch
rpm-build-4.11.13-21.el7.x86_64
libvirt-daemon-driver-qemu-2.0.0-10.el7_3.5.x86_64
[student@CentOS7 ~]$ 

[student@fedora ~]$ sudo dnf list *bzip2*
Last metadata expiration check: …
…
[student@fedora ~]$ sudo dnf install lbzip2-utils
…
[student@fedora ~]$ which lbizp2
/usr/bin/lbzip2
[student@fedora ~]$ sudo dnf remove lbzip2
…
[student@fedora ~]$ 

student@opensuse:-> zypper search gnuplot
…
student@opensuse:-> sudo zypper install gnuplot-doc
…
student@opensuse:-> rpm -qi gnuplot-doc 
…
student@opensuse:-> sudo zypper remove gnuplot
…
student@opensuse:-> 

student@ubuntu:~$ sudo apt-cache search wget2 
…
student@ubuntu:~$ sudo apt-get install wget2-dev
…
student@ubuntu:~$ sudo apt-get remove wget
…
student@ubuntu:~$ sudo apt-get remove wget2
…
student@ubuntu:~$ 

Chapter 8
Finding Linux Documentation 

Use different sources of documentation

Linux documentation sources
Documentation Source
GNU Info
Other documentation Sources
Command help 
The man pages

https://www.gentoo.org/support/documentation/ 

Use the man pages

c7:/tmp>man socket

student@ubuntu:~$ man 7 socket | head -6
student@ubuntu:~$ man 2 socket | head -6
student@ubuntu:~$ man -f sysctl
student@ubuntu:~$ man -k sysctl

c7:/tmp> man -f socket
c7:/tmp> whatis socket
c7:/tmp> man 7 socket
c7:/tmp> man -a socket
c7:/tmp> man -k socket
c7:/tmp> apropos socket
c7:/tmp>  

Access the GNU Info System

The GNU Info System
Info Page Structure
Key      Function
n          Go to the next node
p          Go to the previous node
u          Move one node up in the index

c7:/tmp> info make
/
example
p
u
c7:/tmp>  

Use the help command 

The - -help Option 
C:/tmp> man - -help
C7:/home/coop> help

Use other documentation sources

Desktop help system
Package documentation
Online resources

Chapter 9
Processes 

Describe what a process is 

What is a process ?
                                                               Operating System
Process 1                                                Memory 
Process 2
.
.                                Linux Kernel           CPU
.
.                                                               Physical and 
Process n                                                logical resources 

Process Types


Enumerate processes attributes
Manage processes using ps and top
Understand the use of load averages 
Manipulate processes
Use at, cron, and sleep

Process Type   Description                                                                   Example
  
Interactive        Need to be started by a user, either                             bash, firefox, top
Processes        at a command line or through a GUI

Batch               Automatic process which are scheduled from              updatedb, Idconfig
Processes       and then disconnected from the terminal

Daemons         Server processes that runs continuously                      https, sshd, libvirtd

Threads           Lightweight process. Tasks that run under                    firefox, gnome-
                        the umbrella of a main process, sharing memory          terminal-server
                        and other resources 
Kernel             Kernel tasks that users neither start or terminate           kthreadd, migration,
Threads          and have a little control over                                           lsoftirqd

Process Scheduling and States 
Run Queue
Process 1
Process 2                              Scheduler               CPU
Process 3  

Process and Thread IDs

ID Type                                  Description
Process ID (PID)                   Unique Process ID number 

Parent Process ID (PPID)      Process (Parent) that started this process. If the parent dies,
                                               the PPID will refer to an adoptive parent; on recent kernels, 
                                               this is kthreadd which has PPID=2

Thread ID (TID)                     Thread ID number. This is the same as PID for single-threaded
                                               processes. For a multi-threaded process, each thread shares 
                                               the same PID, but has a unique TID

Terminating a Process
$ kill -SIGKILL <pid>
$ kill -9 <pid>

User and Group IDs

USER IDS                                  USER GROUP IDS
    RUID                                                RGID
Identifies the user                       Identifies the group 
who started the process              that started the process
   
    EUID                                                 EGID
Determines the access                Determines the access
rights of the user                         rights of the group

More About Priorities

c8:/tmp>cat nice.out
…
c8:/tmp>

                          Process 1     Process 2     Process 3  …. Process N
Nice Value        -20                -19                -18
Elapsed Time    0                   1                   2

x7:/tmp> ps
…
x7:/tmp> ps ef
…
x7:/tmp> renice +5 3077
…
x7:/tmp> sudo renice -5 3077
…
x7:/tmp> ps lf
…
x7:/tmp> gnome-system-monitor
…
x7:/tmp> ps lf
…
x7:/tmp> 

Load Averages 
w
top
uptime

student@openSUSE:/tmp> w
…

Background and Foreground Processes

c7:/usr/src/linux> make 0=../linux-7 > /dev/null &
…
c7:/usr/src/linux>

CTRL-Z ( Suspend a foreground job )
CTRL-C ( Terminate a foreground job ) 
bg ( background )
fg  ( foreground ) 

Managing Jobs
c7:/tmp> sleep 100 &
…
c7:/tmp> sleep 100 &
…
c7:/tmp> jobs 
…

The ps Command ( System V Style )

student@ubuntu:~$ ps -ef
…
student@ubuntu:~$

The ps Command ( CSD Style )

c7:/home/coop> ps aux | head -10
…
c7:/home/coop> ps axo stat,priority,pid,pcpu,comm | head -10
…
c7:/home/coop>

c8:/tmp> ps
…
c8:/tmp> ps -f 
…
c8:/tmp> ps -l
…
c8:/tmp>  ps -elf | less
…
c8:/tmp> ps aux | less

The Process Tree

student@ubuntu:~/Pictures$ pstree
systemd    ModemManager        {gdbus}
                                                    {gmain}
                 NetworkManager       dhclient
…
student@ubuntu:~/Pictures$

Top

Command         Output 
t                         Display or hide summary information ( rows 2 and 3 )
m                       Display or hide memory information ( rows 4 and 5 )
A                        Sort the process list by top resources consumers
r                         Renice ( change the priority of ) a specific processes
k                        Kill a specific process
f                         Enter the top configuration screen
o                        Interactively select a new sort order in the process list

c8:/tmp> top
…
c8:/tmp> 

Scheduling Future Processes Using at

c8:/tmp> at now + 2 days 
…
c8:/tmp> # check on schedule job:
…
c8:/tmp> atq
c8:/tmp> # remove the schedule job
…
c8:/tmp> #check
…
c8:/tmp> atq

Cron ( Time based schedule utiliti program ) 

Field         Description         Values 
MIN           Minutes              0 to 59
HOUR       Hour field           0 to 23
DOM         Day of Month      1-31
MON         Month field          1-12
DOW         Day of Week       0-6(0=sunday)
CMD         Command            Any command to be executed 

bob@bobs-computer:/var/spool/crontabs@ sudo cat /etc/crontab

Sleep 

sleep NUMBER [SUFFIX] …

student@openSUSE:/tmp> cat testsleep.sh
…
student@openSUSE:/tmp> ./testsleep.sh
…
student@openSUSE:/tmp> ./testsleep.sh 3
…
student@openSUSE:/tmp> 

Chapter 10
File Operations 

Explore the filesystem and its hierarchy 

Introduction to Filesystems
                                              root(/)
User-1                                   System Files                                          Devices
Data Files                              Compilers                                              Devices
Source Codes                       Scripts                                                    Sound Cards
                                              Binary Files                                            Graphics Cards
/Root ( Usr )



Filesystems Varieties 




Explain the filesystem architecture 

Linux Partitions 
/dev/sda1          EFI System Partition       fat 32    /CENTOS7/…    SYSTEM  260.00 MiB…
 
Mount Points 

                                                              Mount points (/)
                              (/)                                   (/home)                             (/var)
File systems          /dev/sda1/                         /dev/sda5/                       /dev/sda6
                             
                                                                         /dev/sda


$ sudo mount /dev/sda5 /home
$ sudo umount /home 

student@debian:~$ mount | head -10 
…
student@debian:~$ 

Compare files & identify different types

NFS and Network Filesystems

Filesystem  NFS Client
                                            Network                    NFS Server    Filesystem
Filesystem  NFS Client

Overview of User Home Directories 

                      beaver
                  
/home/           wally

                      staff/           ward
                                          
                                         june

/home/faculty
/home/staff
/home/students

The /bin and /sbin Directories 

student@ubuntu:~$ ls -F /bin

The /proc Filesystem 

/proc/cpuinfo
/proc/interrupts
/proc/meminfo
/proc/partitions
/proc/version 
/proc/<Process-ID-#>
/proc/sys

student@openSUSE:-> ls /proc
…
student@openSUSE:->

The /dev Directory 

c7:/tmp> ls /dev
…
c7:/tmp> 

/dev/sda1 ( first partition on the first hard disk )
dev/lp1 ( second printer )
/dev/random ( a source of random numbers )

The /var Directory 

root (/)
          var
              System log files:
              /var/log
                                      Print queues:
                                      /var/spool
                                                          Temp files:
                                                           /var/temp
                                                                          Packages and Database files:
                                                                           /var/lib 
x8:/var> ls -lF
…
x8:/var>

The /ect Directory 

student@debian:/etc$ ls -F
…
student@debian:/etc$

The /boot Directory

vmlinuz
The compressed linux kernel, required for booting.

initramfs
The initial ram filesystem, required for booting, sometimes called initrd, not initamfs

config
The kernel configuration file, only used for debugging and bookkeeping

System.map
Kernel symbol table, only used for debugging 

/boot/grub/grub.conf
/boot/grub2/grub2.cfg

c8:/teaching/LFCW/IMAGES> cd /boot
c8:/boot> ls -l
…
c8:/boot>

The /lib and /lib64 Directories

/lib/libncurses.so.5.9

c7:/> ls -lF lib lib64
…
c7:/>

Removable Media: the/media, /run and /mnt Directories

x8:/run> ls -F /run
…
x8:/run>

/run/media/student/myusbdrive

Additional Directories Under /


Directory Name        Usage 
/opt                           Optional application software packages 

/sys                           Virtual pseudo-filesystem giving information about the system and the     
                                  hardware. Can be used to alter system parameters and for debugging                                                                   
                                  purposes 

/srv                            Site-specific data served up by the system Seldom used

/tmp                           Temporary files; on some distributions erased across a reboot and/or 
                                  may actually be a ramdisk in memory

/usr                            Multi-user applications utilities and data

The /usr Directory tree

Directory Name        Usage 
/usr/include               Header files used to compile applications
/usr/lib                       Libraries for programs in /usr/bin and /usr/sbin
/usr/lib64                   64-bit libraries for 64-bit programs in /usr/bin and /usr/sbin
/usr/sbin                    Non-essential system binaries, such as system daemons
/usr/share                 Share data used by applications, generally architecture-independent
/usr/src                      Source code, usually for the Linux kernel 

/usr/local                   Data and programs specific to the local machine; subdirectories include
                                  bin, sbin, lib, share, include, etc.

/usr/bin                      This is the primary directory of executable commands on the system 

Comparing Files with diff

diff Option                 Usage 
-c                              Provide a listing of differences that include three lines of context before                          
                                 and after the lines differing in content

-r                               Used to recursively compare subdirectories, as well as the current
                                 directory

-i                               ignore the case of letters
-w                             ignore differences in space and tabs (white space) 
-q                              Be quiet: only report if files are different without listening the differences

$ diff [options] <filename1> <filename2>

Using diff3 and patch

$ diffe3 MY-FILE COMMON-FILE YOUR-FILE

c7:/tmp> cat file1
…
c7:/tmp> cat file2
…
c7:/tmp> cat file3
…
c7:/tmp> diff3 file1 file2 file3
…

$ diff -Nur originalfile newfile > patchfile

c7:/usr/src/linux> patch - -dru -run -p1 < /tmp/lab1_syscall_patch 
…
c7:/usr/src/linux>

$ patch -p1 < patchfile
$ patch orifinalfile patchfile

Using the file Utility 

student@ubuntu:~/LFT$ file *
… 
student@ubuntu:~/LFT$

Backing Up Data

cp
someone@host
Rsync

Using rsync

$ rsync -r project-X machine:archives/project-X

$ rsync sourcefile destinationfile

$ rsync - -progress -avrxH - -delete sourcedir destdir

Command           Usage 
gzip                      The most frequently used Linux compression utility
bzip2                    Produce files significantly smaller than those produced by gzip
xz                         The most space-efficient compression utility used in Linux
zip                        Is often required to examine and decompress archives from other
                             operating systems

Chapter 11
Text Editors 

How to create and edit files

Overview of Text Editors in Linux 
                       
                                                   Linux Text Editors
Basic Editors                                                                                                 Advanced Editors
    
nano            gedit                                                                                          vi                emacs       

Creating Files Without Using an Editor
  
$ echo line one > myfile
$ echo line two >> myfile
$ echo line three >> myfile 

$ cat << EOF > myfile
> line one
> line two 
> line three
> EOF
$

nano, a simple text-based editor
Nano is an editor that must be run from a terminal, and focuses on simplicity. Nano is a clone of the old Pico text editor, the editor for the Pine email client, which was very popular back in the 90's on UNIX and UNIX-like systems. Pine has been replaced by Alpine and Pico by Nano, but some things haven't changed - like the simplicity of editing with Nano.

If you don't have Nano, use your package manager to install it, it's in most distro repositories

~nano about.txt

gedit, a simple graphical editor
dedit-factory .c

vi and emacs
~ vim whatisvim.txt 
Vim is a Unix text editor that's included in Linux, BSD, and macOS. It's known for being fast and efficient, in part because it's a small application that can run in a terminal (although it also has a graphical interface), but mostly because it can be controlled entirely with the keyboard with no need for menus or a mouse. For instance, to insert text into a file, you press I and type. To navigate or to issue a command (such as Save, Backspace, Home, End, and so on), you press Esc on your keyboard and then press whatever key or key combination corresponds with the action you want to take. It's a very different way of editing text compared to what modern computer users expect, but it's the way Unix admins all over the world edit config files, changelogs, scripts, and more.

~vimtutor
…

Mode                    Feature 
Command             By default, vi start in command mode
                            Keyboard strokes are interpreted as command that can modify file contents

Insert                    Type i to switch to Insert mode from Command mode
                              Insert mode is used to enter ( insert ) text into a file 
                             Insert mode is indicated by an “? INSERT ?” indicator at the bottom of the
                             screen
                              Press esc to exit Insert mode and return to Command mode
                       
Line                       type: to switch to the Line mode from Command mode. Each key is an 
                             external command, including operations such as writing the file contents to 
                              disk or exiting
                              Press esc to exit Line mode and return to Command mode

Command        Usage 
vi myfile            Start the editor and edit myfile
vi -r myfile        Start and edit myfile in recovery mode from a system crash
:r file2               Read in file2 and insert at current position
:w                      Write to the file
:w myfile           Write out to myfile
:w! file2             Overwrite file2
:x or :wq            Exit and write out modified file
: q                     Quit
:q!                      Quit even though modifications have not been saved 

Key                                Usage 
arrow keys                    To move up, left and right 
j or <ret>                       To move on line down
k                                     To move one line up
h or Backspace               To move one character left
l or Space                       To move one character right
0                                    To move to beginning of line
$                                     To move to end of line
w                                     To move beginning of next word
:0 or 1G                          To move to beginning of file
:n or nG                          To move to line n
:$ or G                             To move the last line in file
CTRL-F or Page Down    To move forward one page
CRTL-B or Page Up        To move backward one page
^l                                      To refresh and center screen

[test3@CentOS ~]$ vi test1
The quick brown fox jumped over the lazy dog.
Nobody expects the Spanish Inquisition !
:wq 
INSERT

[test3@CentOS ~]$ vi test1
The quick brown fox jumped over the lazy dog.
Nobody expects the Spanish Inquisition !

Command          Usage 
/pattern               Search forward for pattern
?pattern              Search backward for pattern 

Key                     Usage 
n                          Move to the next occurrence of search pattern 
N                         Move to previous occurrence of search pattern 

Key                     Usage 
a                          Append text after cursor; stop upon Scape key
A                         Append text at end of current line; stop upon Scape key
i                           Insert text before cursor; stop upon Scape key
I                           Insert text at beginning of current line; stop upon Scape key
o                          Start a new line below current line, insert text there; stop upon Scape key
O                         Start a new line above current line, insert text there; stop upon Scape key
r                           Replace character at current position
R                          Replace text starting with current position, stop upon Scape key
x                           Delete character at current position
Nx                        Delete N characters, starting at current position
dw                        Delete the world at the current position
D                          Delete the rest of the current line
dd                         Delete the current line
Ndd or dNd          Delete N lines
u                           Undo the previous operation
yy                         Yank ( copy ) the current line and put it in buffer
Nyy or yNy            Yank ( copy ) N lines and put it in buffer
p                            Paste at the current position the yanked line or lines from the buffer

Using External Commands in vi

c7:/tmp/s_08> vi lab_miscdev.h
…

[test3@CentOS ~]$ vi test2
Nobody expects the Spanish Inquisition !
Nobody expects the 2020 Revolution !

:wq 
INSERT

[test3@CentOS ~]$ vi test2
Nobody expects the Spanish Inquisition !
Nobody expects the 2020 Revolution !

6 10 80 test2

: ! wc %

Introduction to emacs

#!/bin/bash

Key                      Usage 
emacs myfile        Start emacs and edit myfile
CRTL-x i              Insert prompted for file at current position
CRTL-x s              Save all files
CRTL-x CRTL-w   Write to the file giving a new name when prompted
CRTL-x CRTL-s   Saves the current file
CRTL-x CRTL-c   Exit after being prompted to save any modified files

c7:/tmp> cd /etc/passwd .
cp: overwrite ‘./passwd ? y 
‘/etc/passwd’ -> ‘./passwd’
c7:/tmp> emacs passwd & 
[1] 8279
c7:/tmp>

Query replacing ftp with PTF: (? for help)
Mark set
find file: /tmp/etc/group
Note: file is write protected 

Chapter 12 
User Environment 

Use and configure user accounts 

Identifying the Current User 

student@ubuntu:~$ whoami
student 
student@ubuntu:~$ who
…
student@ubuntu:~$ who

User Startup Files 
                  Shell      
                                 Terminal
/etc 
/home

Order of the Startup Files

~/.bash_profile
~/.bash_login
~/.profile

                           No       .bashrc
Login Shell ?      
                           Yes       .bash_profile 
                                                            .bash_login
                                                                              .profile

Creating Aliases 

student@openSUSE:~> alias 
…
student@openSUSE:~>

Basic of Users and Groups

student@ubuntu:~$ tail -15 /etc/group
…
student@ubuntu:~$ tail -15 /etc/passwd
…
student@ubuntu:~$ 

Adding and Removing Users

useradd
userdel
sudo useradd bjmoose
bjmoose:x:1002:1002::/home/bjmoose:/bin/bash
userdel bjmoose

c7:/home/coop> sudo useradd -s /bin/csh -m -k/etc/skel -c “Bullwnkle J Moose” bmoose
c7:/home/coop> ls -ls /home/bmoose
c7:/home/coop> sudo ls -ls /home/bmoose
…
c7:/home/coop> ls /home
…
c7:/home/coop>

$ id
uid=1002(bjmoose) gid=1002(bjmoose)
groups=106(fuse),1002(bjmoose)

student@ubuntu:~$ less /etc/default/useradd
…
student@ubuntu:~$ sudo useradd -m -c “Eric Dolphy” -s /bin/bash edolphy
student@ubuntu:~$ sudo passwd edolphy
Enter new UNIX password: …
Retype new UNIX password: …
student@ubuntu:~$ grep edolphy /etc/passwd /etc/group
…student@ubuntu:~$ ssh edolphy@localhost
 edolphy@localhost´s password: …
student@ubuntu:~$ ls -la
…
student@ubuntu:~$ exit
…
student@ubuntu:~$ ls -l /etc/skel
…
student@ubuntu:~$ ls -la /etc/skel
…
student@ubuntu:~$ sudo userdel -r edolphy
…
student@ubuntu:~$ ls -l /home
…
student@ubuntu:~$ 

Adding and Removing Groups

$ sudo /usr/sbin/groupadd anewgroup
$ sudo /usr/sbin/groupdel anewgroup
$ groups rjsquirrel
rjsquirrel : rjsquirrel
$ sudo /usr/sbin/usermod -a -G anewgroup rjesquirrel
$ groups rjsquirrel 
rjsquirrel: rjsquirrel anewgroup
$ sudo /usr/sbin/usermod -G rjsquirrel rjesquirrel
$ groups rjsquirrel 
rjsquirrel: rjsquirrel 

The root Account 

#:root 
#:

@dejan@dejan-phoenixnap:~$ sudo -h

su and sudo

Elevating to root Account 

stunde@openSUSE:~> ls -la /root
…
stunde@openSUSE:~> sudo ls -la /root
student´s password: …
stunde@openSUSE:~> 

Use and set environment variables 

c7:/tmp> env | head-5
…
c7:/tmp> set | head-5
…
c7:/tmp> export | head-5
…
c7:/tmp> 

Setting Environment Variables 

Task                                      Command 
Show the value                     echo $SHELL
of a specific variable 
 
Export a new variable            export VARIABLE=value(or VARIABLE=value;
value                                      export VARIABLE)

Add a variable permanently   Edit ~/.bashrc and add the line export VARIABLE=value
                                               Type source~/.bashrc or just ~/.bashrc(dot ~/.bashrc); or just
                                               start a new shell by typing bash

$ SDIRS=s_0* KROOT=/lib/modules/$(uname -r)/build make modules_install

The HOME variable

student@ubuntu:~$ echo $HOME
/home/student
student@ubuntu:~$ cd usr/bin
student@ubuntu:~$ /usr/bin$ pwd
/usr/bin 
student@ubuntu:~$ /usr/bin$ cd $HOME
student@ubuntu:~$ pwd
/home/student
student@ubuntu:~$
 
Command                   Explanation 
$ echo $HOME           Show the value of HOME environment variable , the change 
/home/me$ cd/bin       directories (cd) to /bin

$ pwd                          Where are we? Use print (or present) working directory (pwd) to 
/bin                              find out. As expected, /bin

$ cd                             Change directory without an argument …

$ pwd                          … take us back to HOME, as you can now see
/home/me 

The PATH variable

student@ubuntu:~$ echo $PATH
…
student@ubuntu:~$ OLDPATH=$PATH
student@ubuntu:~$ PATH=$PATH:/opt/some_application
student@ubuntu:~$ echo $PATH
…
student@ubuntu:~$ 

:path1  :path2
path1::path2

$ export PATH=$HOME/bin:$PATH
$ echo PATH /home/student/bin:/usr/local/bin:/usr/bin;/bin/usr

The SHELL variable

$ echo $SHELL 
$

Use the previous shell command history

The PS1 Variable and the Command Line Prompt

chris@ubuntu:~$ DEFAULT=$PS1
chris@ubuntu:~$ PS1=“/u/$”
…
chris@ubuntu:~$

\u - User name
\h - Host name
\w - Current working directory
\! - History number of this command
\d - Date 

student@openSUSE:~> echo $PS1
…
student@openSUSE:~> OLDPS1=$PS1
student@openSUSE:~> PS1=‘\u@\h:\d\w>’
student@openSUSE:~> Wed Dec 14~>cd /tmp
student@openSUSE:~> Wed Dec 14/tmp>PS1=$OLDPS1
student@openSUSE:~> 

Recalling Previous Commands

student@debian:~$ history | tail -20
…
student@debian:~$ 

Using History Environment Variables

HISTIFILE : The location of the history file
HISTFILESIZE: The maximum number of line in the history file(default 500)
HISTZINE: The maximum number of commands in the history file
HISTCONTROL: How commands are stored
HISTIGNORE: Which command lines can be unsaved 

c7:/tem> set | grep HIST
…
c7:/tem>

Finding and Using Previous Commands

Key                                            Usage
Up/Down arrow keys                 Browse through the list of commands previously 
!!(Pronounced as bang-bang     Execute the previous command
CTRL-R                                      Search previously used commands

Use keyboard shortcuts 


Keyboard Shortcut          Task

CTRL-L                            Cleans the screen
CTRL-D                            Exists the current shell
CTRL-Z                             Puts the current process into suspended background
CTRL-C                            Kills the current process
CTRL-H                             Works the same as backspace
CTRL-A                             Goes to the beginning of the line
CTRL-W                            Deletes the world before the cursor
CTRL-U                             Deletes from beginning of line to cursor position
CTRL-E                            Goes to the end of the line
Tab                                   Auto-complete files directories, and binaries  

Use and define aliases 

…

Use and set files permissions

File Ownership

Command         Usage

chown               Used to change user ownership of a file or directory
chgpr                 Used to change group ownership

chmod               Used to change the permissions of the file, which can be done separately 
                          for owner, group and the rest of the world(often named as other)



$ ls -l somefile 

-rw-rw-r- - 1 student student 1601 Mar 9 15:04 somefile
$ chmod uo+x,g-w somefile 
$ ls -l somefile
-rwxr- -r-x 1 student student 1601 Mar 9 15:04 somefile



$ chmod 755 somefile
$ ls -l somefile
-rwxr- -r-x 1 student student 1601 Mar 9 15:04 somefile

Example of chwon and chgpr

c7:/tmp> touch file1 file2
c7:/tmp> ls -l file ?
…
c7:/tmp> sudo chwon root file2
c7:/tmp> ls -l file ?
…
c7:/tmp> sudo chwon root:root file?
c7:/tmp> ls -l file ?
…
c7:/tmp> rm file ?
…
c7:/tmp> sudo rm file ?
c7:/tmp>

c7:/tmp> touch file1
c7:/tmp> ls -l file1 ?
…
c7:/tmp> chgrp bin file1
c7:/tmp> ls -l file1 ?
…
c7:/tmp> rm file1
c7:/tmp>

Chapter 13
Manipulating Text

Display and append to file contents

Command Line Tools for Manipulating Text Files 

student@debian:~$ tail etc//services
…
student@debian:~$ cat etc/services | sort | uniq | awk ‘{print $1}’ | tail
…
student@debian:~$ 

Edit and print file contents 

cat ( Concatenation )

$ cat <filename> 
$ cat readme.txt 

Command               Usage
cat file1 file2            Concatenate multiple files and display the output; i.e. the entire content 
                                of the first file is followed by that of the second file

cat file1 file2 >         Combine multiple files and save the output into a new file
new file

cat file >>                Append a file to the end of an existing file
extingfile

cat > file                  Any subsequent lines typed will go into the file, until CTRL-D is typed  

cat >> file                Any subsequent lines are appended to the file, until CTRL-D is typed

$ tac file
$ tac file1 file2 > newfile

cat > <filename> 

stundent@ubuntu:/tmp$ rm -f file*
stundent@ubuntu:/tmp$ nano file1.txt
and I will just 
type in a couple
of lines 
stundent@ubuntu:/tmp$ cat file1.txt
and I will just 
type in a couple
of lines 
stundent@ubuntu:/tmp$ cat << EOF > file2.txt
> here is a second
> file with a few
> lines
> EOF
stundent@ubuntu:/tmp$ cat file2.txt
here is a second
file with a few
lines
stundent@ubuntu:/tmp$ cat file1.txt file2.txt
and I will just 
type in a couple
of lines 

here is a second
file with a few
lines
stundent@ubuntu:/tmp$ cat file1.txt file2.txt > file3.txt
stundent@ubuntu:/tmp$ cat file3.txt
and I will just 
type in a couple
of lines 

here is a second
file with a few
lines
stundent@ubuntu:/tmp$ 
Working with Large Files

$ less somefile
$ cat somefile | less

Head

student@ubuntu:~$ head -15 /etc/default/grub
…
student@ubuntu:~$ 

$ head -n 5 /etc/default/grub
$ head -5 /etc/default/grub

Tail

$ tail -n 15 somefile.log
$ tail -15 somefile.log
$ tail -f somefile.log

student@ubuntu:~$ tail -15 /etc/default/grub
…
student@ubuntu:~$ 

Search for patterns 

Introduction to sed and awk

Sed

Input Stream - > Working Stream - > Output Stream 

[student@fedora~]$ cat /etc/sysconfig/man-db
…
[student@fedora~]$ sed e s/yes/no/g /etc/sysconfig/man-db
…
[student@fedora~]$ 

Command                                    Usage
sed -e command <filename>        Specify editing commands at the command line, operate
                                                     on file and put the output on standart out (e.g. the terminal)

sed -f scriptfile <filename>           Specify a scriptfile containing sed commands, operate on 
                                                     file and put output on standard out 

echo “I hate you” | sed                  Use sed to filter standard input, putting output on standard
s/hate/love/                                   o

Command                                     Usage
sed s/pattern/replace_string/        Substitute first string occurrence in every line 
file        

sed s/pattern/replace_string/g file       Substitute all string occurrences in every line 

sed 1,3s/pattern/replace_string/g file   Substitute all string occurrences in a range of lines

sed -i s/pattern/replace_string/ g file    Save changes for string substitution in the same file

[student@fedora tmp]$ cat infile.txt
This is the first line
This is the second line
This is the third line
[student@fedora tmp]$ sed -e s/is/are/ infile.txt
Thare is the first line
Thare is the second line
Thare is the third line
[student@fedora tmp]$  sed -e s/is/are/g infile.txt
Thare are the first line
Thare are the second line
Thare are the third line
[student@fedora tmp]$ sed -e 1,2s/is/are/g infile.txt
Thare are the first line
Thare are the second line
This is the third line
[student@fedora tmp]$  sed -e 1,2s:is:are:g infile.txt
Thare are the first line
Thare are the second line
This is the third line
[student@fedora tmp]$  sed -e 1,2s:is:are:g infile.txt > outfile.txt
[student@fedora tmp]$ cat outfile.txt 
Thare are the first line
Thare are the second line
This is the third line
[student@fedora tmp]$ diff infile.txt outfile.txt
1, 2c1, 2
< This is the first line
< This is the second line
- - -
> Thare are the first line
> Thare are the second line 
[student@fedora tmp]$ 

Awk

student@Linux-Mint-18 ~ $ head -10 /etc/passwd
…
 student@Linux-Mint-18 ~ $ awk -F: ‘{print “name: “$1” shell:” $7} ’ \
…
student@Linux-Mint-18 ~ $ 

Command                                Usage 
awk ‘command’ file                   Specify a command directly at the command line
awk -f scriptfile file                    Specify a file that contains the script to be executed

Command                                Usage
awk ‘ { print $0 } ’                      Print entire file
/etc/passwd

awk -F: ‘ { print $1  } ’               Print first field (column) of every line , separated by a colon
/etc/passwd

awk -F: ‘ { print $1 $7 } ’            Print first and seventh field of every line 
/etc/passwd

Use multiple other utilities 

File Manipulation Utilities

Sort 

c8:/etc/default> cat grub
…
c8:/etc/default> 

Syntax                                Usage
sort <filename>                   Sort the line in a specified file, according to the character at the 
                                            beginning of each line

cat file1 file2 |                      Combine the two files, then sort the lines and display the output 
sort                                      on the terminal

sort -r <filename>               Sort the lines in reverse order

sort -k 3 <filename>           Sort the lines by the 3rd field of each line instead of the beginning

Uniq

student@openSUSE:/tmp> sort uniqdemo.txt
…
student@openSUSE:/tmp> sort -u uniqdemo.txt
…
student@openSUSE:/tmp> 

sort file1 file2 | uniq > file3
sort -u file1 file2 > file3 
uniq -c filename

Past

-d 
-s

c7:/tmp> cat phone
…
c7:/tmp:> cat names
…
c7:/tmp:> past phone names 
…
c7:/tmp:> past -d ‘:’ phone names
…
c7:/tmp:> 

$ past file1 file2 
$ past -d, file1 file2

Join 

$ join file1 file2

c7:/tmp:> cat phonebook
…
c7:/tmp:> cat cities
…
c7:/tmp:> join phonebook cities
…
c7:/tmp:> 

Split
                                                                  Each file with 1000 lines
File with more            split infile                 Each file with 1000 lines
than 1000 lines                                          Each file with 1000 lines 

$ wc -l american-english
99171 american-english
$ split american-english dictionary 

student@ubuntu:/tmp$ wc /usr/share/dict/american-english
…
student@ubuntu:/tmp$ split /usr/share/dict/american-english dictionary 
student@ubuntu:/tmp$ ls -l dictionary* | wc 
…
student@ubuntu:/tmp$ ls -l dictionary* | head -10
…
student@ubuntu:/tmp$ 

Regular Expressions and Search Patterns 

[^]*?@[^]*?\.[^]*

Command             Usage

a..                          matches azy
b. | j.                       matches both br and ju
..$                          matches og
l.*                           matches lazy dog
l.*y                         matches lazy
the.*                      matches the holy sentence 

Grep

Command                                 Usage 

grep [pattern] < filename>         Search for a pattern in a file and print all matching lines

grep -v [pattern]                         Print all lines that do not match the pattern
<filename>

grep [0-9] <filename>                 Print the lines that contain the numbers 0 through 9

grep -C 3 [pattern]                      Print context of lines ( specified number of lines above and 
<filename>                                 below the pattern ) for matching the pattern. Here, the 
                                                   number of lines is specified as 3

Strings

$ strings book1.xls | grep my_string

student@ubuntu:/usr/bin$ strings a* | grep GPL
…
student@ubuntu:/usr/bin$  

[student@FC-25 tmp]$ cat trinput | tr ‘a-l’ ‘A-L’ > troutput
[student@FC-25 tmp]$

[student@FC-25 tmp]$ head -20 trinput
…
[student@FC-25 tmp]$

[student@FC-25 tmp]$ head -20 troutput
…
[student@FC-25 tmp]$

$ tr [options] set1 [set2] 
$ cat city | tr a-z A-Z 

Command                                       Usage 

tr abcdefghijklmnopqrstuvwxyz       Convert lowercase to uppercase    

tr ‘{ }’ ‘{ }’ < inputfile> outputfile        Translate braces into parenthesis 

echo “This is for testing” |               Translate white-space to tabs
[:space:] ‘\t’  

echo “ This  is  for  testing ” tr -s      Squeeze repetition of characters using -s
[:space:] 

echo “The geek stuff” tr -d ‘t’            Delete specified characters using -d option 

echo “my username is 432234” |      Complement the sets using -c option 
tr cd [:digit:]   

tr -cd [:print:] < file.txt                        Remove all non-printable character from a file

tr -s ‘\n’ ‘ ‘ < file.txt                             Join all the lines in a file into a single line

Tee

c7:/etc> sudo find . -name “g*cfg” | tee /tmp/tee_output
…
c7:/etc> cat /tmp/tee_output
…
c7:/etc> 

$ ls - | tee newfile

WC

c7:/usr/src/linux/kernel/sched>wc *h
…
c7:/usr/src/linux/kernel/sched>

Option                          Description
  
-l                                   Display the number of lines
-c                                  Display the number of bytes
-w                                  Display the number of words

Cut

c7:/tmp> cat tabfile
…
c7:/tmp> cut -f2 tabfile
…
c7:/tmp> 

$ ls -l | cut -d“ ” -f3

Chapter 14
Network Operations 

Explaining basic network concepts

Introduction to Network

Allow devices communication 

Local Network                                                          Internet 
Computer                           Router
Laptop           Internal IPs                  External IP 
Cellphone

Enable device sharing

IP Address

172.20.161.0        Cloud            157.28.162.2

IPv4 
32-bit address
4.3 billion possible addresses
Example: 192.0.1.246

IPv6
128-bit address
340 undecillion possible addresses 
Example: 2002:db8::8a3f:362:7897

Share and manage information

10.0.01
10.0.0.2        Router + NAT ( Network Address Translation )      Server 200.100.10.10
10.0.0.3            200.88.1.11
Devices behind
the router with
private IP
addresses 



Configure network interfaces and use utilities 

Decoding IPv4 Addresses 

Example 
IP Address     172          .     16       .          31.         46
Bit format       10101100.00010000.00011111.00101110

Class A Network Addresses

An example of a Class A Address is: 

10                 .       233          .           45            .        23
00001010     .   11101001     .     00101101      .    00010111

Octet 1               Octet 2                Octet 3                Octet 4
0                         HOST ID              HOST ID            HOST ID
Net ID

Class B Network Addresses

An example of a Class B Address is: 

135                 .      201           .           18            .        1
1000111         .   11001001     .     00010010      .    00000001

Octet 1               Octet 2                Octet 3                Octet 4
1 0                                                  HOST ID            HOST ID
        < - Net ID - >

Class C Network Addresses

An example of a Class C Address is: 

192                 .      33              .            84          .          156
11000000       .   00100001     .     01010100      .    10011100

Octet 1               Octet 2                Octet 3                Octet 4
1 1 0                                                                          HOST ID
    < -                  Net ID                      - >

IP Address Allocation

Allocation IP Addresses
Manually       Dynamically  
Static IP        Dynamic Host
                      Configuration Protocol

140.211.169.4
Server IP Address of
Linux foundation
www.linuxfoundation.org

More Networking Tools

student@ubuntu:~/Desktop$ cat /etc/resolv.conf
…
student@ubuntu:~/Desktop$ cat /etc/hosts
…
student@ubuntu:~/Desktop$ ping Rodrigo
…
student@ubuntu:~/Desktop$ host Rodrigo
…
student@ubuntu:~/Desktop$ host linuxfoundation.org 
…
student@ubuntu:~/Desktop$ nslookup linuxfoundation.org
…
student@ubuntu:~/Desktop$ dig linuxfoundation.org
…
student@ubuntu:~/Desktop$ 

Network Configuration Files

Debian Version 
/etc/network/

Red Hat and SUSI family
/etc/sysconfig/network/

Network Interfaces

c7:/tmp> ifconfig eno1
…
c7:/tmp> ip -s link show eno1
…
c7:/tmp> ip address show eno1
…
c7:/tmp>  

The IP Utility

$ /sbin/ip addr show
$ /sbin/ip route show

c7:/home/coop> ip addr show
…
c7:/home/coop>

Ping

$ ping <hostname>

c8:/tmp> ping -c 10 linuxfoundation.org
…
c8:/tmp>  

Route 

student@ubuntu:/etc$ route -n
…
student@ubuntu:/etc$ ip route
…
student@ubuntu:/etc$ 

Task                                            Command
Show current routing table          $ route -n or ip route
Add static route                           $ route add -net address or ip route add
Delete static route                       $ route del -net address or ip route del

Traceroute

c7:/tmp> traceroute www.linuxfoundation.org
…
c7:/tmp> 

More Networking Tools

Networking Tools             Description
ethtool                              Queries network interface and can also set various parameters 
                                         such as the speed

netstat                              Displays all active connections and routing tables; useful for 
                                         monitoring performance and troubleshooting 

nmap                                Scans open ports on a network; important for security analysis 

tcpdump                           Dumps network traffic for analysis

iptraf                                 Monitors network traffic in text mode

mtr                                       Combine functionality of ping and traceroute and gives
                                             a continuously updated display

dig                                        Tests DNS workings; a good replacement for host and nslookup

Using more Networking Tools

test1@ubuntu:~$ sudo ethtool eth0
…
test1@ubuntu:~$ netstat -r
…
test1@ubuntu:~$ sudo nmap -sS 10.0.2.15/24 
…
test1@ubuntu:~$ 

Use graphical and non-graphical browsers

Firefox
Google Chrome
Chromium
Opera
Vivaldi

Non-graphical         Description
Browsers

lynx                         Confgurable text-based web browser; the earliest such browser and still
                                in use

elinks                       Based on Lynx; it can display tables and frames

w3m                        Another text-based web browser with many features

Wget

c8:/tmp> wget https://training.linuxfoundation.org/cm/prep/ready-for.sh
…
c8:/tmp> 

Curl

c7:/tmp> curl -o lf.html https://linuxfoundation.org
…
c7:/tmp> 

-> ~ curl https://www.freecodecamp.org
…

$ curl -o saved.html http://www.mysite.com


Transfer files to and from clients and servers 

SSH: Executing Commands Remotely 

                                                     Internet
                                                   SSH Tunnel

SSH                                                                                                 SSH
Client                                                                                              SERVER
machine C                                                                                     machine S

                                                                                            Mail Server

$ ssh_some_system
$ ssh -l someone some_system
$ ssh someone@some_system
$ ssh some_system my_command
 
Copying Files Securely with scp

scp <localfile> <user@remotesystem>:/home/user/

Using SSH Between Two Virtual Machines

student@ubuntu:~$ ip - -brief addr show 
…
student@ubuntu:~$  ssh student@172.16249.129
…
student@ubuntu:~$  exit
…
student@ubuntu:~$ cd /tmp
student@ubuntu:/tmp$ ls -l student
…
student@ubuntu:/tmp$ 


[student@centos ~]$ ip - -brief addr show
…
[student@centos ~]$ scp -r /home/student 172.16.249.133:/tmp
…
[student@centos ~]$ 





