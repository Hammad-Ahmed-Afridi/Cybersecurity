# Try Hack Me
## Cybersecurity 101
- offensive security red teaming pentesters are basically methodologies and individuals that
  hack a system in an ethical legal way to find flaws and weaknesses and vulnerabilities
  before a real attacker does and for this first you need to understand the system find the
  vulnerabilities and then exploit them in websites first in order to find hidden or all the
  directories or web pages we use the dirb domain or url or use the gobuster tool with
  command: gobuster dir --url http://www.onlineshop.thm/ -w /usr/share/wordlists/dirbuster/
  directory-list.txt and when a secret page is found that can give privilage level or give
  some sort or administrator role we exploit that by either bruteforcing the password or
  do a dictionary attack for dictionary attack we use hydra for passwords if the admin name
  is know : hydra -l admin -P passlist.txt www.onlineshop.thm http-post-form "/login:username
  =^USER^&password=^PASS^:F=incorrect" -V first they do enumeration that is finding and
  gethering information related to the system this process is done by both the red teamers
  are black hat hackers
- defensive security blue teaming and methodologies used for defending and protecting a system
  against malacious actors they maintain the  cia triad methodology and for this they have
  to first understand the system and then secure it from hackers and monitor the activity in it
  they prevent detect and mitigate attacks
- shodan is the tools used as a browser for iot devices like it deals with all the devices that
  have a public ip and scans them for open ports servers gives details to them like versions
  countries
- virustotal is a tool that lets user scan a file a url a domain against 70+ known virus
  detection engine adn scanners that will flag the input and give off the malacious factor
  score
- cve common vulnerability and exposure is a database for all the known vulnerabilities in
  this database their are vulnerabilities with naming as cve-year-unique number we can check
  cves and their cvss commom vulnerability scoring system in cve official website nist nvd
  national vulnerability database and also for proof of concepts and exploit codes we can use
  github which also has detailed technical reports for a cve 
- in linux if a user wants to get details about a cerrtain tool or commad they use man or -h
  for it like man toolname/command or toolname/command -h man stands for manual and h stands
  for help we can alos use whatis command/toolname
- Linux is basically an os kernel that was built by linus torvalds and it was bundled with
  GNU softwares and packages to create an os called GNU/linux which is basically the parent os
  for all the distributions that are existing today like ubuntu debian kali linux rhel fedora etc
  for root actions we use the keyword sudo and then the command and tehn it will ask fo for the
  password and then the actions will be performed for the local user
- now some bash commands
  ``` bash
  systeminfo  // in cmd for system details
  help  // we can use the help command before the command
  cls  // for clearing the screen
  ipconfig /all  // for network related details
  ping domain or ipaddress  // for pinging a network to check the connection
  tracert ipaddress  // traces the route that was used to reach the destination
  netstat -abno  // for deatiled output related to connections
  echo hello world  // give us the output on the screen
  whoami  // tells us about the current user
  ls  // lists all the files and directories in the current folder
  ls -al  // listing the hidden files and folders also starting with the . operator that the system hides by default also give file permission info
  cd foldername  // change the directory to teh name mentioned
  cd ..  // goes back one directory
  cat filename  // outpust the text in the file on the screen
  pwd  // prints working directory or current directory
  find -iname "filename.txt"  // finding the file in a directory and i is for ignoring the case of the alphabets
  find / -name "filename.txt"  // finding the file in teh entire system / stands for root
  find -name *.txt  // the wildcard is used for finding all the files with the .txt extension
  find . -type d -name "directory name"  //  . for searching within active directory or ~ for home directory or / for root directory
  touch filname  // to create a file
  mkdir foldername  // making a new directory 
  echo "hello"  // to write content
  echo "text" > filename or >>filename
  nano filename  // used for booting the text editor
  rm filename  // delating a file
  rm -rf foldername  // deleting a folder
  ssh username@ipaddress  // secure shell use logout for terminating the session
  su - root  // for root access
  su - username  // switching users also type logout for logging out
  history  // command for checking the command typed in the past
  man command or toolname  // use for manual pages
  command or toolname -h or --help  // used for help
  cp file1 file2  // used for file and folder copying first is to be copied and second is the location
  mv file1 file2  // used for file and folder copying first is to be moved and second is the location
  file filaname  // gives the filetype forexample text or image
  chmod 444 file.txt  // uses the file permission and the file is read only for everyone including the group and the owner
  scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt
  scp ubuntu@192.168.1.30:/home/ubuntu/documents.txt notes.txt
  python3 -m http.server
  wget http://MACHINE_IP:8000/myfile
  apt search toolname
  apt update  // we can put toolname with it also for specifying it
  apt upgrade  // same here
  apt install toolname
  apt remove toolname
  apt purge toolname
  ```
- we use & and then the command to make the process run in the background and use fg to make the
  background processes come in the foregroud also we use && to type multiple commands in a single
  line we use > operator for writting text to a file and that deletes the pre written text in it
  and >> operator for writing text with the pre writtin text like it does not delete it
- we use ssh secure shell to remotely adn securely connect to a linux machine using encryption
  it lets us execute commands on the remote machine and the sent data is encrypted over the internet
- file or folder permissions and rwxrwxrwx that is read write execute the first is for the owner the
  second is for the group and the third is for the whole world r has teh value of 4 and w has the value
  2 and x has the value of 1 and for each bock it adds up we use these numeric values in chmod command
  in which we give and take permissions to a specific file chmod is change mode
- common directories like /etc that has /etc/passwd for user info and /etc/shadow for user login
  credentials that are salted and hashed then we have /var that has information about system logs and
  usage var stands for variable then we have /root which is the home directory for root user and then we
  /tmp stands for temporary it has temporary data just like ram has that system uses 
- terminal editors include the nano which we get using the nano command and the filename and vim
  we use wget webpage url to download the webpage we are currently on our local machine only the html
  part for downloading the images and style as well use wget -p -k https://example.com and for
  downloading the entire website we use wget -m https://example.com and the gets downloaded in the same
  folder we used the command in we use the scp for  copying files between the source and destination using
  ssh the command is mentioned in the bash section then we have python3 which we use to either make out host
  or other remote machine a webserver and download files on the machine we use commad python3 -m http.server
  in the folder we want the files to be downloaded and then on the other machine use the wget command
  wget http://MACHINE_IP:8000/myfile
- processes are programs running on the machine they have their specific id known as PID and the pids are
  given in systematic order like first 0 is given then 1 then 2 then 3 and so on the processes can be seen
  using ps aux or top command the pid 0 goes to the first process that boots after the pc turns on that is
  systemd and this is the parent process from which all other child proecss comes out we can kill a process
  using kill command and then the pid also we can start stop enable or disable process at the boot using
  systemctl start apache
- we use cronjobs for scheduling a task in linux we use the command crontab -e for adding the task and use
- crontab -l for checking the cronjobs the systematic way of writing a cronjob is * * * * * command
  the first area is for minute that is 0-59 the second is for hour that is 0-23 the third is for day of the
  month that is 1-31 the fourth is for month of the year that is 1-12 and the last is day of the weak that is
  0-6 0 is the sunday and so on we can use shortcuts as well with the @ sign like @reboot @daily @weekly
  @monthly and then type command in this way we dont have to write the full 5 fields and also the hash sign
  shows comments in the crontab
- for package management or software downloads we use apt advanced package tool for searching downloading and
  updating the packages and tools in the machine
- GUI graphical user interace that lets us use the softwares and applications on our system effortlessly
  in order to connect to a remote desktop turn on the rdp on remote machine setting - system - remote desktop
  then get the ip from the remote machine and also the account username anad password and the either use the
  dialogue box for remote desktop connection type mstsc or use cmd
  ```bash
  mstsc /v:ipaddress
  ```
- we have NTFS new technology file system that brings new features like encryption larger file holding faster
  file and folder permissions that FAT and HPFS high performance file system did not brought in the c directory
  we have windows folder that holds the windows operating system and in that folder we have a critical most
  important folder called system32 folder 
- for managemnet for the entire system like all the user account file folder and devices and equipments and other
  controls just type cmd or dialogue box and type compmgmt.msc and for control panel type control panel for user
  account control just open dialogue box and type useraccountcontrolsettings and just move the pointer to which
  security you want for checking performance of the system and check the apps running and also check about cpu ram
  we use task manager and the dialogue box prompt is taskmgr
- for opening absolutely every feature like the oned mentioned above we can use MSconfig in cmd or dialogue box
  windows update windows defender firewall windows security virus and threat protection we have bitlocker that is
  used for full drive encryption and file encryptions as well and the uses sysmetric encrytion and then the keys are
  stored in tpm trusted platform module which is a hardware device that actually checks for anomalies in the hardware
  before booting up like first we turn on the power button the uefi/bios turn on the hardware and then tpm checks for
  anomalies if not found it gives away the encryption decryption keys so that the folders or files can be decrypted
  that were done by bitlocker the keys are handed over to cpu and when decryption of the main folder occurs like the
  wiindows folder the other happens as we go the then os kernel takes control booting up the os itself and then it lets
  users interact with software and applications using hardware
- we have windows domain that is the entire bubble for the active directory and that domain is like the website domain
  with a . in it also having subdomains we have that windows domain that is stored in a server called windows domain
  server which becomes a domain controller and whoever is the the administrator of the server is the domain administrator
  and the administrator of the entire active directory then in the domain we have multiple users devices computers and we
  put them in organizational units in the form of objects so that we can apply a set of rules called group policies to
  them we use ad for a broader network of devices or users and we use compmgmt for a single computer management
- we use delegation to give some users access over other ous so that they can control them or help them like IT people
  helping other users for system errors changing passwords
- for creating and managing group poicies we use group policy managemnet becasue we can not use active directory for this
  and then drag that specific policy in gpo to the desired ou
- for authentication over active directory we use kerberos and ntlm for sso ntlm is outdated the new method is kerberos
  kerberos is like this first the user logs in his system and then what happens is the password is not forwarded what happens
  is the username is sent and the timestamp is encrypted using the key derived from the password and then it is sent to AS
  authenticating server and then the server responds with tgt ticket granting ticket and that tgt is used by the host whenever
  using a service like when using a service on his system instead of again typing in username and password for the service
  like he did for log in signup what happen sis the tgt + the service is sent to tgs ticket granting server and then it hands
  over the ticket to the host and that ticket is then used for accessing the services NTLM got rolled out because it does not
  do mutual authentication as kerberos do and the host blindly trusts the server
- we have domains as discussed earlier than if we have multiple subdomain for a single domain we have a tree for it like under
  a domain tree we have subdomains like a main domain that is domain.com and then we have two subdomains servers and 2 ads
  first.doimain.com and second.domain.com each one has its own domain controller and both of them are controlled by a single
  domain controller then we have forests that is if we have multiple domains like domain.com and hello.com these when connected
  to a single administrator forms a forest and as both are on different domain in a forest they need to have a trust relationship
  whether that is one way or two way so that both the domains can get use and access the other domain services 
- to switch between cmd or powershell just type the one you want and press enter use the tree command for
  a proper visual representation of directories in a path for making or removing a diorectory use mkdir and rmdir
  for creating file use type nul > file.txt and for writiing use echo and for printing use type filename for
  process running and pids we use tasklist the command to shutdown pc shutdown /s for restarting shutdown /r
- powershell is a shell or cli that is object oriented that is built on .NET framework and the commands are known
  as cmdlets command lets main cmdlets we have verb-noun combination like get-content for printing content
  set-location for changing directories get-command for getting all the cmdlets for getting command that starts with
  specific verb like we want to have remove commands we use get-command -name remove* get-help get-content will print the
  properties and usage and help us in getting the grasp of get-content cmdlet or others then we have alias that is
  when used it gives us the commands that we used in bash and give its alternative cmdlets get-alias we use pipping
  so that we can use two commands together like first one does the operation and the second one does the operation
  on the output and it done by using the | symbol get-childitem | where-object -property length -eq 100 where eq
  means equals to also we can use ne lt le gt ge get-computerinfo get-localuser get-netipaddress
- we can rdp to a windows or ubuntu when xrdp is installed on linux using the mstsc command in windows and when
  connecting from linux to windows we use the internel tool called remmina and then use rdp details to connect to
  it also we can use ssh for all shells bash powershell or cmd also a command for ssh through a specific port
  ssh -p 443 username@ipaddress
- scripting is basically a process in which we save commands in a file and then use them by using those files in the
  future for powershell we use the extension .ps1 and for bash we use .sh and for cmd we use .bat or .cmd
  for scripting in bash first create a file using nano than give executable permission using chmod +x then inside
  the file use she bang #!/bin/bash and then type commmands like echo then use the read name to input name from user
  then use if else like if["$name"="ali"]; then echo " " else echo " " fi and then in order to run it use ./filename
  also for using comments use #
- OSI model stands for open system interconnection is a conceptual model developed by international organization for
  standardization it tells us hwo packets move from one device to another in a network that is internet we have
  seven layers layer 7 is application than we have presentation than session than transport than network than datalink
  and than physical when we go from layer 7 to layer 1 we have encapsulation happening that is packets are covered in
  envelops and in each layer we have extra packets added on top of each other and in the data link layer we call the
  packet frame which is the exception and when we move from layer 1 to 7 decapsulation occurs 
- layer 7 is the layer we use like the interface which allows us to interact with the digital world this layer deals with
  protocols like http ftp dns smtp than we have presenation layer that makes our interaction and our inputs
  understandable to the devices on the network that is it converts it into machine readable like its use ascii or unicode
  than we have session layer that creates manages and destroys session between devices on a network ssh or telnet and than we have
  transport layer that uses the session to transport the packets to the desired destination and the protocols used are
  tcp and udp and than we have network layer that transports or delivers the packets to devices on different networks connected
  using routers they use ip addresses and the protocols used are ICMP OSPF and RIP than we have data link layer that deals
  with packets called frames and this layer sends frames using switch between devices on the same network using mac addresses
  than we have physical layer that deals with physical connections like wires ethernet cables or wifi ethernet cables include
  cat 5 cat 6 cat 7 cat 8 and the thing that is connected to the end of it is called registered jack RJ 45 and we have two types
  of cables straight through and crossover cables straight are for different devices and crossover are for same devices 
- than we have tcp/ip model developed by us dod and it is a practicel model consisting of 4 layers application layer is the forth
  than the transport layer and the the network layer and than the data link layer we also for conviniece use five layers
  that is application transport network datalink and physical
- we have subnetting that is deviding an existing network in to multiple smaller networks called subnet and these subnets are called
  vlans virtual local area network we have a subnet mask for 192.168.1.0 is 255.255.255.0 that is also denoted by /24 at the end of
  ip address what this shows is that we can create a subnet on the network 192.168.1.0 ranging from 1-254 bacause these are usable ips
  and in these numbers the ip address 192.168.1.1 is the deafault gateway that is the address used by the router to connect to the
  outside network and ip address 192.168.1.255 is the broadcast address that is this address is used bu the router for sendding
  packets to the entire network devices such that im ARP subnetting happens at the switch level that is layer 2 and a router is
  required or at layer 3 switch where no router is required for subnetting what we do is first we take a single layer 2 switch use
  it do create different vlans like subnets one is 192.168.1.0 and the othe ris 192.168.2.0 and then connect both these vlans to a
  single switch and in order for them to communicate to each other and to the outside network we use a router and connect that single
  switch to a router and we can reduce the number of devices by taking out the router and use a layer 3 switch instead
- we use private ip address for local network devices that is each device on the local network gets a private ip and that local network
  when connected to a router gets a public ip to use the internet that public ip is of router and the router use NAT to let the private
  ips use a single public ip but lets say we do not have a router connected to the switch what happens is the ip addresses get assigned
  automatically so that the devices could communicate to each other but they can not communicate to the internet
- DHCP dynamic host congiguration protocol uses DHCP server to assign an ip to a device on a network it is a series of four steps
  that is DHCP discover that is a packet sent by the device using the ip address 0.0.0.0 to the broadcast address 255.255.255.255 to
  discover a DHCP server on the network than the serevr responds using a DHCP offer offering a ip address than the device sends a DHCP
  requuest for requesting the usage of the ip address and than the server responds by DHCP acknowledge and then the ip address is used
  by the device the process is DORA discover offer response acknowledge and we use the DHCP server for gaining both the public and private
  ips one server is local one and the other one is internet service provider owned
- ARP address resolution protocol is a protocol used for getting trth emac address of a device of which only the ip is known what happens is
  when two devices are connected in a network they get ips from dhcp server but in order to communicate between each other they must know
  each other mac addresses so in order to know the mac of the destination device the sourse device sends a arp request packet on a broadcast
  mac address ff:ff:ff:ff:ff:ff to the entire network stating which mac address has the known ip address the ip address is know like
  192.168.1.1 and then the device that has that ip sends an ARP reply stating that i am the device that has ip 192.168.1.1 and have this mac
  address and this information gets stored in a table called arp tables 
- icmp is used for network trouble shooting this is used by ping commad that we use with an ip address for checking whether a device on a
  network is responding or not
- NAT network address translation is a process used by routers for masking the private ips of devices on a network and allowing them to
  use a single public ip for internet or communication outside the network 
- we use ssl/tls secure socket layer or transport layer security for secure encrypted communication over the internet and we use digital
  certificates issued by certifing authorities cas to authenticate ourselves or are used by the servers to authenticate themselves
  when accessing the web or web apps we can not every time use our login credentials to authenticate ourselves so what happens is that our
  browser has a certificate store that has all the signed certificates of the root cas so what happens is when we make request the server
  sends its own certificate which is signed by the certifying authority and when that certificate reaches the browser the browser checks the
  signature and when matched the resource is accessed and used
- when the certificate is to be issued what happens is the server requests the ca for a certificate and that certificate gets stored in the
  certificate database with its own ttl and also when in usage the client sends its ca to a device and then that device uses the public key
  of that ca that has given the certificate and decrypts the signature and when the signature matches the signature in the local trust store
  its authenticates it because the machine trusts what ca trusts the decryotion is done the output is a hash and also when the client browser
  does the hashing to the certificate of that ca in its own trust store and then match it to the decrypted server sent certificate whose output
  was a hash for actual authentication and whenever the intermediate ca is not matched it then goes up teh chain of root ca to check and match
  its certificate this whole process is called chain of trust and the certificate attaining process is called certificate issuence and the
  authentication process is basically decryption and hashing process 
- nowadays we use https which uses tls certificate for secure encrypted communication over tcp port 443 and we can check this by running wireshark
  and whenever a certain website is visited first we will have the tcp 3 way handshake with the server and then it will establish a tls
  connection and then whatever is sent over the connection will be encrypted and when we open a certain paccket it will be gibberish text like
  we wont know what is written some important https request are get post put delete
- for most of the time for our convinience we can say in most of the protocols if s is behind it it means it is using ssh like sftp and when it is
  at the suffix position it means it uses ssl like https smtps ftps pop3s 
- wireshark tool you can learn it from youtube by taking a short crash course it is so easy to grasp as you have the knowledge for it and all
  the things mentioned above and the things that you will be seeing in that tools basically that tool gives to packets that are travelling over
  the network its has all the details like the protocols used ports used sequences packet body which is mostly encrypted if the protocol used
  is the secure one the ssl tls one we can save the wireshark packets captured as a file having the extenssion or format as .pcapng that stands
  for packet capture next generation or .pcap we can use wireshark to capture real time traffic by running the blue shark fin button or use the
  packets capture saved file we can view the packet details by just clicking the single packet and we will get the details like protocols prots
  ips macs headers body and the encrypted text which is encoded also we can go to specific packets by putting in the packet number in the
  go search bar we can also find the desired packets by name as well we can also use filters by just filtering tem in the filter search box from
  names ips protocols or other things and we will get the desired filter output only ignoring the rest and all these features are at the top
  of the wireshark gui we can also apply colours to packets for our ease of use which will show us the problems false positives critical etc
- as mentioned earlier wireshark is a gui tool and most of the systems in servers and clouds dont support gui so we need a tool to capture and
- analyze packets and asve them so that we can view them in wireshark after that in the form of .pcap files we can use the command
  ```bash
  tcpdump -i ens5 -c 5 -n
  ```
  here the i stands for the interface and c stands for the number of packets to be captures and what n does is it do not let domains and ports to
  resolved in simpe readable text like we want actual ips not domains names of servers or systems for more detailed output we can add -v at the end
  we can also apply filters in the form of host filters port or protocol filters and also we can read and write .pcap files in it
  ```bash
  tcpdump host example.com -w http.pcap
  tcpdump -i ens5 port 53 -n
  tcpdump -i ens5 icmp -n
  tcpdump -r TwoPackets.pcap
  ```
- nmap is a tool used for scanning the network for live hosts for open ports and many other services bash commands
  ```bash
  nmap -sn 192.168.66.0/24  // for scanning the entire subnet
  nmap -sn 192.168.66.0  // for scanning the single ip
  nmap 192.168.66.0/24  // for scanning 1000 most common ports on the entire network
  nmap -p 22,80,443 192.168.66.0/24  // for specific port scans we can also specify the ports from 1-65535 after -p
  nmap -sT 192.168.66.0/24  /// for tcp ports
  nmap -sU ip  // for udp ports
  nmap -sS -sV -O 192.168.124.211  // we use sv for service and version detection and o for os detection
  ```
- cryptography is basically scrambling data using an alogorithm so that its confidentiality is maintained and also the scrambled data is
  called cipher text and in order to read it again we can use a key to bring it back to readable format this process is called encryption
  and decryption historic ciphers include ceasar cipher which shifts the text letters using the key as the base than we have rot 13 also we have
  transposition cipher which inncludes keyless and keyed ciphers and vigenere cipher we have two types of encryptions that are symmetric and
  asymmetric encryption symmetric encryption uses a single key for both encryption and is also called private key cryptography or encryption and
  asymmetric ecryption uses public and private key for cryptography public key and private key public key used for encryption and private key for
  decryption and is called public key cryptography 
