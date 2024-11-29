## Basics

> type <command>  (user for getting details of command is that internal or external)
	Ex- type echo

> pwd (print working directory)

> pushd  /etc

> popd

> more <file_name> (see data in file)

> less <file_name> (see data in file)

> whatis <command> (get details of what this command is used for)
	Ex - whatis cat

> man <command>  (get full details of command)

> apropos <command>  (get list of all commands that  matches to this name)

> env (list all environment variables)

> echo $SHELL (print which shell we are using)

> chsh (for changing shell)

> alias dt=date

> history

> which <command> (get location of command)




> export PATH=$PATH:/opt/obs/bin
	(Save path to environmental variable)


> uname (print kernel of system)

> uname -r (print version of kernel)

> sudo dmesg (print all messages of kernel)

> udevadm info --query=path --name=/dev/sda5

> udevadm monitor

> lscpu  (list information of CPU)

> lsmem --summary (list memory information of CPU)

> free -m (it’s useful to show total vs free memory in the system)

> lshw (detailed hardware configuration)

> lsblk

> df -hP

Two type of package manager 
DPKG / APT (Debian package manager)  => apt/apt-get (advance package manager)
RPM		=> yum

> du <file_name> (shows file name with size of file)

> du -sh text.img (print size of file in mb)

> tar -cf <tar_file_name> <file_name_1> <file_name_2> ..
		(Create tar file of this file as mentioned)

> tar -tf demo.tar (list all files inside tar file)

> tar -xf test.tar (uncompress tar file)

> tar -zcf demo.tar (compress tar file) 

> locate <file_name> (find file in linux file system)

> updatedb (update local file database)

> find <file_name> (find file in database)

> grep <world> <file> (find name in file)




## NETWORKING


> ifconfig

> ip <address> 

> traceroute <destination> (list all ip addresses between route)

> tracepath <destination>

> ping <destination> (connectivity between two node)

> netstat (print list of open sockets , routing table, connection info)

> ss (replacement of netstat)

> dig <domin_name> (get detail of DNS)

> nslookup <domainName> (get detail of DNS / replacement of dig /replacement of ping)

> wget <file_url> (get content from internet like downloading file)

> curl <file_url> (get content from internet like downloading file same as wget)

> mtr <destination> (combination of ping and traceroute)

> whois <website> (get all information of website)

> ifplugstatus (get is cable connected to server or not)

> iftop (used for traffic monitoring)

> tcpdump (Linux tcpdump command is the most used command in network analysis among other Linux network commands. It captures the traffic that is passing through the network interface and displays it.)