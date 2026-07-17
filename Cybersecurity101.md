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
  sha256sum filename.txt  // for hashing a file 
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
  examples include AES DES BLOWFISH asymmetric ecryption uses public and private key for cryptography public key and private key public key used
  for encryption and private key for decryption and is called public key cryptography examples include RSA DSA DEFFIE HELLMAN ECC 
- hashing is used for checking data integrity and data realness hashing is used for storing passwords as passwords can not be stored in raw form
  in databases so first they are hashed and then they are stored and whenever user inputs password it get hashed and then it is matched with the
  stored hash and if they match the user is authenticated but now adays due to attacks where hashes are brute forced using rainbow tables salting
  is used in which a salt that is a random string is added to the password and then it is hashed and stored so that the password can not be
  guessed in this way even if the password is in the rainbow table and is also guessed the attacker can not get autheticated bbecasue of the salt
  it changed the hash completely and this is a property of hashing that a small change in input can cause a very large change in output and this
  is called avalanche effect now discussing about file integrity hashing is also used their when we download something from the internet what
  happens is that the website give us a hash of the original file so that we could check against it by hashing the downloaded file on our own
  system if the hashes dont match we will get to know that their was some sort of tempering done to the file and it is not secure we can not reverse
  a hash we can just guess the real password and hash it and then match it to the hash and this is done using tools like john the ripper or hashcat
  in linux password hashes are stored in /etc/shadow file and for cracking them first we have to unshadow them using the unshadow command in a .txt
  file and then use john the ripper or hashcat and use a wordlist like rockyou.txt which contains the most common passwords each hash tells us
  what algorithm is used what salt is used and what is the actual hash and each segment is seperted by a $ sign we have different hash functions
  like sha1 sha256 sha512 yescrypt bescrypt 
- we have a tool called metasploit that checks a system or a network against known vulnerabilities and also for confirmation create and execute
  exploits for accessing and using the vulnerabilites and then using payloads for further actions let us say i have a server in my home lab or
  in the network i want to check it against known server vulnerabilities i will first check the open ports or services running on it by using nmap
  and its ip address nmap -sV 192.168.1.X we can use the nmap inside the metasploit frameword we can run the framework by just typing msfconsole
  as we have discovered teh services and ports on the server we can use teh metasploit for finding specific vulnerabilties realated to the service
  running then use that to scan against it and check if the service or server is vulnerable or not and if yes we use the msfvenom which is
  metasploit meterpreter to develop an exploit and use the payload for a complete attack and control 
- we have websites and webapps that are opeened in browsers and we can interact with them made from html css javascript as frontend frameworks and
  languages and for backend we use php python java javascript and fro databases we use sql or nosql databases the componenst of the websiet or
  webapps are stored or deployed on a web server and also their are many other compinenets like cdn cache waf dns we can access resourses on the
  browser or internet using urls uniform resource locater first it shows the protocol then the actual domain then port number then the path to that
  specific resource then the queries strating from ? then the additional fragments we have different methods to interact with websites and webapps
  like get post put and delete get fetches teh resource delete deletes it post adds new resouce and put updates the resource whatever we do on teh
  browser we are always requesting resources from teh web server and teh server is responding and this is called http request and response and
  in these messaeges we have header and body which contains many type on info which is easy to guess their are also status codes when we deal
  with websites like 404 page not found 200 ok and 500 server error
- stuctured query language is a language used to create read update delete and perform crud and other operations on a relational database
  first of all we have to run my sql in cli using the command "mysql -u root -p " u for user that is root and p for password in order
  to create a database we use "CREATE DATABASE databsename;" in order to look at all the created databses we use "SHOW DATABASES;" in order to
  use a specific database we use "USE databsesname;" and if we no longer need a databse we use "DROP DATABASE databasename;" as we have created
  a databse we have to create tables in it for storing content that are related as it is a relational database "CREATE TABLE tablename (
  example_column1 data_type, example_column2 data_type, example_column3 data_type);" for checking different tables in a databse we use "SHOW TABES;"
  and if we want to get a look at the table we created we use the "DESCRIBE tablename;" if we want to alter a table like adding or deleting something
  we use "ALTER TABEL tablename and then use a specific command after that;" and then for dropping that we use "DROP TABLE tablename;" now as the
  databse and tables are created we have to perfoem crud operation create read update delete for creatig new record in the table we use INSERT INTO
  command and then tyep the rest of the command for reading we use SELECT and if we want to select everything like read everything we use * after
  SELECT and then use FROM and then type the table name for example SELECT * FROM tablename; and if we want to be specific we can use
  SELECT coloumnname FROM tablename; for updating a record in the table we use the update command for example UPDATE tableaneme and the use the rest
  of the command; for deleting something we use DELETE FROM tableanem and the use the rest of the commands; 
- burpsuite is a tool used for web pentesting it sits as a proxy between a browser and web server and captures every packet and allows us to alter
  them according to our needs and also allow us to perform attacks on the website or webserver like xss sql inject xsrf authentication bypass and
  other attacks as well it is a gui tool that is used to find vulnerabilities in a website and exploit them 
- Hydra John the Ripper and Hashcat are industry-standard tools. Hydra is for online brute-forcing testing live login pages/services) while John
  the Ripper and Hashcat are for offline cracking recovering plaintext from stolen or extracted password hashes
- gobuster is used for directory enumeration and for subdomain enumeration for enumerating directories we use the following command
  ```
  gobuster dir -u "http://www.example.thm/" -w /usr/share/wordlists/dirb/small.txt -t 64
  gobuster dir -u "http://www.example.thm" -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -r
  and for enemurating sub directoories we use the following command
  gobuster dns -d example.thm -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt
  ```
- for sql injection we have manual method in which we add a username and then type a random password and add some random characters to it as well
  which results in autentication like in password area we can type :  'abc' OR 1=1;-- -';  the OR operator will do a trick which is
  that abc will give the password wrong but 1=1 is always true and will give true which will lead to attack but this process is slow and for
  fast attacks we use a tool called sqlmap   the ultimate sqlmap command
  ```
  sqlmap -u "http://target.com" --batch --level=5 --risk=2 --random-agent --dbs  // thsi will find the databse names
  sqlmap -u "http://target.com" --batch -D databsename --tables  // this will give all the tables in te found database 
  sqlmap -u "http://target.com" --random-agent --forms --level=5 --risk=3 --dump --batch  // this is the aggressive prompt that will dumo everything 
  ```
- SOC security operations centre is a department which monitors and safeguards the entire organizatgion against malacious activities and attacks
  their main job is do monitor detect respond contain eradicate and gain knowledge and prevent future mishaps and apart from incident response
  they also do forensics as well they consist of soc analyst l1 soc analyst l2 soc analyst l3 security engineer detectgion engineer and above them
  is the soc manager and then the ciso when ever the soc team is triaging alerts they answer these 5 question who what when where why the technology
  that is used in soc is siem security information and event management which is a tool that centralizes logs of different devices on the
  organization network into a single interface and after the attack is contained and eradicated forensics is done how firstly all the logs are
  gathered which are mere activities on the devices and then the relevent ones are seperated analyzed and then a report is created which containes
  how the attack happened what vulnerabilty was their how was it exploited and how the attacker gained access and did lateral movements and did
  privilage escalation and also recommend how to prevent such type of attack in the future the attacks are merely inciidents like every adversary
  action or any other action that can or is causing harm to the network or system is an incident and gets logged in the siem solution their are
  somme false positives which are ignored or removed but the true positives are teh ones that are focused on the actions that are followed by the
  soc team for prepariing and eleminating attack is basically a framework provided by SANS and NIST 
- Siem security information and event management is a tool used for centralized log monitoring and alerting from different sources suign built in
  tools like forwarders or agents we can also manually add logs in the siem solution and what it does is correlats logs find patterns and helps in
  alert triaging as in modern times ai is also implemented for more accurate alerts and for more complex relations in siem solution alerts
  are generated when a specific rule is violated these rules are created by security engineers and their are two types of alerts false positives and
  true positives
- firewall are either hardware devices or software that monitors the inbound and outbound traffic and allow or deny them using rules created
  their are types of firewalls like stateless and statefull and proxy and next generation firewall stateless firewall just allows or blocks
  packets based on rules but do not keep the state of connections statefull firewalls allow and block based on rules as well as keep state of
  connections that are stable or unstable and allow or block connections as well then we have next generation firewalls that are quite complex
  in terms of security and also quite useful in bigger infrastructure in windows we have windows defender firewall and in linux we have uncomplicated
  firewall in windows we can simple use it using the gui but in linux we haev to use it in cli we can allow deny connections to certain ports
  enabel disable rules or firewll as a whole whenever we are creating a rule in firewall we always need the source ip destination ip port
  portocol action like allow deny forward and at last the direction like inbound or outbound inbound is the traffic that is comming in the
  network and outbounnd is the traffic that is going out of the network 
- IDS intrusion detection system basically datects intrusions in a network or a system firewalls are for monitoring the tgraffic going in and out
  but what if the attacker or malacious packet gets past the firewall so their must be some sort of way to detect this intrusion and for this we
  use IDS their are two types of IDS network based NIDS and host based HIDS and the detection is of two types signature based and anomaly based
  in signature based IDS the device has all the signatures of malicious packets and viruses malwares that exist signatures are strings that
  define a certain virus or malware but these IDS are not good against zero day attacks so we use anomaly based IDS which checks and trains itself
  by looking at normal network connections and network working and when a small change happens it detects it and in modern times hybrid IDS are
  used we haev an open source IDS called snort it is a hybrid tool and it has pre built rues in it and we can also add custom rules as well
  we can add rules in /etc/snort and use following command in cli
  ```
  alert icmp any any -> 127.0.0.1 any (msg:"Loopback Ping Detected"; sid:10003; rev:1;)
  ```
- vulnerabilties are weeknesses or gaps or flaws in a system or network or software that can be exploited by a threat actor and this can be
  prevented by patching it or by updating or disabling usused services it we can perform these scans internally from inside the network or
  externally from outside the network authenticated or unauthenticated their are many tools for vulnerability scan nessus qualys nexpose
  openvas open vulnerabilty assessment system which is an open source vulnerabilty assessment tool openvas is a gui tool which is installed
  first with its dependencies using docker and then run in browser and peroform the actions and it will show the vulnerabilities against
  knows cve common vulnerabilities and enumerations cve number is given to every vulnerabilty with a year and random number in the form of
  CVE - 2024 - 68492 also we have a CVSS common vulnwrabilty scoring system which tells us about the severity of the vulnerabilty 
- cyberchef is the cybersecurity swiss army knife it is browser based tool that has many features like ecryption decryption for different
  algos hashing using differnet hash algos encoding decoding using differnt bases annd many more tools like obfuscation etc
- CAPA common analysis platform for artifact is a tools used for analysis static or dynamic in static analysis the artifact that is a file
  analysis is done without running or executing it and dynamic analysis is done using running or executing the artifact for running
  capa on a certain file we use the command
  ```
  capa.exe filename
  ```
  this will give all the data related to file like hashes os path it will also give us ATTACK which is attack tactics techniques and common
  knowledge which is a frame work provided by MITRE corp which gives us details about the attacks taht happened how they were performed all
  the techniques used by the adversary
- security principles are frameworks that are created which then are used by organizations to create their own security
  policies so that their asserts could be protected nothing can be 100 percent secure or protected but the effort could be made to minimize the
  loss or attacks happening CIA triad confidentiality integrity availability we also have authentication and auditing/accountabilty and non
  repudiation the opposite of cia is DAD disclosure Alteration and Destruction/Denial we have some famous security models that are bell lapadula
  model bibas model and clark wilson model in bell lapadula model we have three variations simple star and strong star in simple it is no read up
  in star it is no write down and in strong star it is no read up no write down the security model has different security clearance levels and rules
  are applied to them this model focuses on confidentiality then we have bibas model it also has three variations in simple we have no read down
  in star we have write up and in strong star we have no read down write up for different security levels this model focuses on integrity and then
  we have clark wilson model which focuses on integrity of data inn which their are two types of assets or data which can be accessed in two different
  ways first one can be accesssed directly without any authentication authorization but the other secure type can be accessed by going through
  different clearance levels and then allowed to access it 
- Defence or security is not a single layer to be applied it is a series of steps and a series of layers to be implemented that will provide the
  neccessary protection to the infrastructure and this is defence in depth whenever we are defending a system we have to keep these things in mind
  that are authentication authorization access control non repudiation confidentiality integrity redunduncy least privilage patching removing
  unneccessay services auditing or monitoring we have polp which is principle of least privilage that is granting access to resources so that
  the entity can perform just the actions it is allowed to do for completing the job not mmore that that and we have zero trust that is never trust
  always verify even the entities within an infrastructure 
- vulnerabilties are weaknesses gaps or logical flaws in a system and threat is the actor that can exploit the vulnerabilty and risk is the
  probability that the threat may exploit and take advantage of that vulnerabilty 
- Red team acts as an ethical hackers they use real world hacker tactics like phishing physical security breaches and malware emulation to uncover deep              vulnerabilities missed by standard engineering providing actionable data for VAPT (Vulnerability Assessment and Penetration Testing) reports blue
  acts as the defender they design secure systems maintain security controls monitor network traffic for anomalies and actively respond to incidents
  to mitigate both real and simulated attacks.
