# Try Hack Me
## Presecurity
- dirb command used for finding hidden directories and pages on a website using `dirb` command
  ```bash
  dirb https://websitename.com
  ```
- booting the pc involves pressing the power button then the power supply unit distributes the
  power to the components than the basic input output system BIOS or unified extensible firmware
  interface (both of these connect the hradware to the operating system) checks for any anomaly
  with the hardware componenets then it finds the os in the storage either HDD or SSD and then
  initiates the bootloader which boots the os and computer turns on completely
- BIOS is the older version and in modern times UEFI is used which is a firmware that is a low
  level software
- Computers are everywhere tabs laptops smartphone iot devices and embedded systems
- Client server model in which client requests a service from the server which responds to it by
  delivering it
- we have protoccols which basically is how computers communicate with each other and then we
  have ports that are hardware and software both and they are used at network endpoints and
  application endpoints and then we have DNS which is domain name system that translates user
  entered domain name to computer readable url or domain then we have http and https which are
  web protocols that are used for communicating and https is used for secure communication
  then we have status codes like 200 OK 403 Forbidden 404 Page not found and we can find all
  this information related to domain requests and server responses by inspecting the page and
  going to network section
- virtualization is a technology that makes small isolated compartments in a computer that has
  its own os cpu ram memory allocated so that the computer or the server can be utilized in a
  maximum way these isolated compartments are called virtual machine and this technology is
  possible through hypervisor which is a virtualization software and we have type 1 and tyep 2
  hypervisors tyep 1 is used in servers and type 2 is used in computer pcs makes a single
  computer act like multiple computers
- containeriation is also a technology used for isolation but instead of having its own os it
  uses the host os kernal and packages everything for apps to run in isolation and is achieved
  through docker
- we use hypervisor for virtualiation in a server or a system by creating virtual machines
  and then use containerization for making small isolated conatiners in those vms
- cloud computing is basically renting out compute storage that is servers by not actually
  owning the hardware the hardware belongs to big tech companies and companies just rent out
  spaces for cost effectivness backups security redunduncy uptime reliability we have IAAS PAAS
  SAAS we have public private and hybrid cloud
- we have the operating system that sits between the hardware and the applications that lets users
  interact with the applications and lets application use the system resources like cpu ram
  storage then we have os kernel that is the core of os that basically handle the system
  resource management user management process manangement we have os for everypurpose like for
  personnel computers mobiles servers etc we have cli which is the command line interface for
  windows we have cmd and powershell and for linux we have bash bourne again shell or terminal
  the user have the highly privilaged unrestricted access in windows is called administrator and
  in linux is called root
- now some bash commands
  ```bash
  pwd prints current directory
  cd change directory
  for moving one directory back cd ..
  ls list content
  ls -al list hidden content that os hides by default starts with the . operator
  find finds the file or folder file . or ~ or / -name filename file / -type d -name directory
  touch to create a file
  echo to write content to file echo "text" > filename
  nana filename used also
  deleting a file or folder rm filename rm -r foldername
  whoami for checking the user
  ssh username@ipaddress
  for root access jjust type su - root
  when logged in and want to switch user su - username
  history command for checking the command typed in the past
  ```
- some cmd commands
  ```cmd
  cd instead of pwd
  cd for changing directory as well
  for moving one directory back cd ..
  dir instead of ls
  dir /a instead of ls -al
  dir /s instead of find
  type instead of cat
  ipconfig
  whoami
  systeminfo
  ```
- CIA triad that is confidentiality integrity availibility confidentiality is securing or
  protecting against unauthorized access integrity is protection against unauthorized change
  and availibilty is the data or information or resources available using backups and
  redunduncy access control is basically the process of controlling who gets to use what
  principle of least privilage polp is allowing activities or actions to users that will
  let them do their intended tasks or work without giving any other allowences malware is
  the malicious software virus worms trojans rootkist logic bombs ransomware
- bits are 0 and 1 one bit can have one of te two values 1 or 0 and in a byte we have 8
  bits rgb red green blue used for making other colurs each colour has 256 different
  intensities which gives 256x256x256 colours 16.7 million we have binary base 2 decimal
  base 10 octal base 8 and hexadecimal base 16 0-9 A-F 
- ascii american standard code for information interchange is used for data or character
  encoding for english characters and numbers but for other languages it was not present
  iso did the work for creating the encoding ascii schemes for other languages as well but
  still there was issue that users sent something else and other user after decoding got
  something else so we got unicode that replaced the legacy ascii scheme which gave an
  encoding characters to each character in every languaage and then unicode uses the
  unicode transformtion format utf8 utf16 utf32 to convert it to binary so that computers
  can use and store it unicode is also used for emojis as well
- network are devices connected together we have private network and public network
  internet is a giant network connectoing many small networks together creator of world
  wide web tim berners lee public network is internet and private is intranet 
- we have ip address and mac address internet protocol is a
  4 octet number like 192.168.1.1 having 0-255 variations for each octet this is ipv4
  the ip address is given by the techniques called ip addressing and subnetting
  we needed ipv6 because number of devices on the internet were growing and this address
  can never be same for two devices on a single network so we need ipv6 address that is
  represented by aaaa:2222:2222:4444:bbbb:gggg:4444:3333 we have media access control
  address which is the permanent address of a device which is and can be connected to a
  network or internet because of a nic network interface ccard it has on its motherboard
  the address is like a4:b5:74:v5:9h:gg the first six digits gives us the manufacturer who
  built the nic and the last six digits give us the host numebr which is unique mac
  addresses can be stolen and changed by spoofing that is making another device use the
  mac of one device and act like it
- we have ping command which uses internet control messsage protocol packet icmp to ensure
  devies connected to the network are sending and receiving packets without any hindrance
  and it also checks or gives us time taken in milliseconds
  ```bash or cmd
  ping (ipaddress or domain name)
  ```
- lan topologies that is the design of a network we have star bus and ring topology in star
  all the devices are connected to the centre hub or switch which is a device that connects
  different devices on a netwrok using the ethernet technology or cables (RJ45 rigistered
  jack) cat5 cat6 cat7 cat8 the older version of switch was repeater which was dumb that forward
  the packets to every device on that network in bus topology the devices are connected to a
  single backbone that is a wire or a connection in ring topology every device is connected
  to one another in a ring like 1 is connected to 2 and 2 is connected to 3 and 3 is then
  connected to 1 in this way if one connection breaks the entire network goes down and if
  one device is sending the traffic then it can not receive traffic then we have router which
  connects different networks together switchs and router both have ports  and routers direct
  traffic within network and switches direct traffic within devices we have modem that brings
  the internet from isp to a comapany and then we have router that connects different networks
  within that company than we have swicth that connects different devices together to form a
  network and in modern routers we have modems prebuilt and also they have wap as well
  modem modulator demodulator
- ip addresses and assigned through a techniques known as subnetting using a subnet mask that
  is deviding a network into smaller networks in ipaddress 192.168.1.1 we have the network
  address 192.168.1.0 and then the host address is from .1 to .254 and the broadcast address
  .255 and the default gateway is either one of the host address
- ARP address resolution protocol which sends a packet using the braodcast address to the
  entire network that which mac address has this ip address and then the device with that
  specific ip responds that it has that mac address and then it is stored in cache for
  future use ARP request ARP reply
- ip addresses are assigned to devices either manually or through a DHCP server dynamic
  host configuration protocol server first when device connects to a network it is either
  an ip address manually or sends a DHCP discover request packet on the network and then when
  DHCP server is present it sends a DHCP offer that this ip is available then the device
  sends DHCP request and the DHCP server DHCP acknowlodge packet and then the device starts
  using the ip address
- rj45(this is the plastic connecter at the end of the cables) ethernet cables are of two
  types straight through cables and crossover cable straight through used for connecting
  different devices in a network and crossover is used for connecting same devices in a network
  a cable has 8 wires twisted together in pairs of 4 we have cat5 cat6 cat7 cat8 (category)
  the cables are twisted so that the data loss is reduced and interferance is also reduced
- OSI open systems interconnection model developed by iso is a conceptual model or
  framework for networking is a netgworking model that tells us how data is
  sent and received over the network and this model has seven layers 7 application
  6 presentation 5 session 4 network 3 transport 2 data link 1 physical data moving
  from layer 7 to layer 1 is encapsulated that is more data is added and when in reverse it
  is decapsulated layer 7 application is the software side the apps we use and work on that
  show us data that got received and also from here we send the data as well layer 6
  presentation is the layer responsible for making that data transferable and useable over
  a network layer 5 session is the layer that manages to construct and maintain connection
  between the sender and the receiver systems and is alos responsible for cutting the
  connection as well layer 4 is the transport layer is the layer that uses the session
  established and transport the data or packets over the network using tcp or udp
  tcp transmission control protocol which is relaible and safe use tcp three way handshake
  synchronize synchronize/acknowledge and acknowledge steps udp user datagram protocol
  is fast but not relaible as data can get lost layer 3 is the network this layer actually
  directs the traffic over to the desired destination network over an entire system of
  networks using protocols like ospf open shortest path first and routing information
  protocol layer 2 is the data link layer which receives teh packets from the layer 3 and
  adds mac addresses using the arp protocol to check which mac has this ip so that packets
  could be transfered to desired destination layer 1 is the pysical layer that deals with
  physical aspects of the networking that is hardware which include RJ45 ethernet cables
- packets are chunks or prices of data or informatio sent over a network and frames
  is basically packet within a packet that is when encapsulation occurs more data is
  added to packet and the packet is wrapped around another packet and that packet is
  called frame in packet we have source and destination ip and in frame the source
  and destination mac addresses are also added
- ports are of two types hardware and software hardware ports are pockets or sockets
  in a system that connects to ethernet cables or hdmi cables so that other devices
  could be connected to it or used by it and software ports are virtual ports
  ranging from 0-65535 are endpoints that allow the internet traffic to be directed
  to the desired destination or interface or application they act as doors to the
  internet traffic common ports ssh22 ftp21 telnet23 http80 https443 protocols are
  standards set that the computers use when communicating with each other and over
  the internet
- port forwarding lets a private network make its system or systems public by
  opening up specific ports or ports to the public internet so that anyone over a
  different network use the services of that private network and this is acheived
  in routers firewalls are either softwares or hardwares but both have the same
  function managing what traffic gets allowed in the network and gets to go outside
  network they are of two type stateless which have pre defines rules and only acts
  on those rules like blocking packets that are malacious and statefull that also
  have predefined rules but they are smart not dumb like the stateless they monitor
  the entire network connection and blocks not only the packets but also the
  connection if found malacious 
- vpn virtual private network lets devices across different networks connect to each
  other securely as they are physically present their and that connection is secure
  encrypted and not visible to the people over the internet except the isp provider
  this is helpful if an office is located far from the main office and the sub office
  wants to use the resources or systems of the main office like servers computers 
- routers are layer 3 networking devices that do routing managing packet transmission
  over the network and choosing the most reliable most safest and most fastest path
  over the network using protocols like ospf or rip then we have switches which can
  be managed or unmanaged which are layer 2 and layer 3 networking devices on layer
  2 they deal with mac addresses and on layer 3 they dela with ip addresses as well
  we use routers for subnetting which is nwtwork segmentation proccess and we use
  switches layer 2 for vlan virtual local area network when doing vlan segmentation
  we devide a single switch into two or three virtual switches having that become
  isolated from each other and needs a router to send and receive the packets just
  like 2 seperte switches connected to each other through a router we can also use
  two seperate switches as well for vlan we have on public ip that is used by router
  and for vlan 1 we will have 192.168.1.0 as network adddress and 192.168.1.1-254/24
  as host address and .255 as the broadcast address and .1 as default gateway and
  for vlan 2 we will have 192.168.2.0 as network adddress and 192.168.2.1-254/24
  as host address and .255 as the broadcast address and .1 as default gateway
- DNS domain name system lets us use the services over the web by translating our
  website request to ip address like domain name to ip address www.google.com to
  8.8.8.8 domain heirarchy is root-tld top level domain-sld second level domain
  subdomain root(.) tld(.com,.edu,.gov,.ca,.uk tld is of two types cctld(country
  code) gtld(generic)) second level domain is the domain in which another part is
  added before the tld like google.com and subdomain is the part added the left of
  sld using a . operator like sites.google.com dns record types are A for ipv4
  addresses AAAA for ipv6 addresses 
- first request is made and is checking in the local os and browser cache if found
  the service is provided if not the request is forwarded to recursive dns server
  provided by isp which also checks if it is present in its cache if not the request
  is forwarded to the root server which checks the tld and forward it to that
  specific tld server which also forwards it to the actual server that holds all the
  records to that specific domain and then after that the dns record is stored in the
  local browser or so cache as well for future use with time to live ttl and the
  browser gets the ip address for that specific server which it will use for making
  the actual request
- http is a protocol used for requesting and delivering html over the web and its
  secure version is https that encrypts the traffic for requesting a server for
  a website or some other web service we use url uniform resource locater that has
  protocol then the domain name and then the port number than the path and the some
  quesries with a question mark sign and then some fragments witha hash sign we have
  methods and the four main methods are get method which is used for retreiving
  information then we have post method used for putting new information on the server
  then we have put method for updating old information on the server and then we have
  delete method for deleting information on the server we then have status codes
  which show us what happened with our request and what happened with the servers
  response 200-ok 404-page not found 403-forbidden 503-service unavailable then we
  have headers that have additional data for the server when request is made
  containing cookies content length content type host then their are header responses
  sent by the server to the client containing set cookie cookies are small pieces of
  data that are sent by the server so that it can authenticate a person whenever the
  service is used by that person and the server sends the cookie data in the form of
  set cookie that gets stored in the cookie storage this happens because http is stateless
  and in order to remember the user and its activity without the need for authentication
  again and again cookies are used which are forwarded to the server upon request and has ttl
- how web works first we request the website on browser and then the request gets sent over
  the internet and then to the server and then the server responds with the website which 
  gets shown on the browser the website the made up of html css javascript in the code the
  developer may have left some sensitive information which can be used by the attacker for
  unauthorized actions html injection displays text or code on the front end when the input
  sanitization is not implemented like not checking or blocking what user entered and
  accepting it as it is
- first the domain name is types in the browser and the dns server looks up and returns the
  ip address for that domain and then the request is sent to the server over the internet and
  then the response is presented on the browser we also have some other technologies in
  between this request and response which is load balancers which sits between the serve and
  the response and manages the traffic what it does is use algorithms to direct the traffic
  to the least busy server so that the up time is not effected and clients can use the
  services without any hindrance like round robin or weighted they also do health checks on
  the servers as well than we have cdn content delivery network what it does is instead of
  string a website or web app on a single server it stores copies of it on multiple servers
  over the entire globe and when a user requests the service the request is sent to the most
  nearest server possibble for fast responses and minimal load then we have databases that
  store information so that it can be accessible over the internet then we have waf web
  application firewall that sits between client and server and protects the server from
  malacious activities like ddos distributed denial of servic or malacious packets or ips
- web servers stores web services like websites webapps and when a request is sent or received
  by the server from the internet it delivers the desired requested service to the client on
  the internet the web server is hardware that is the physical black machine and then it has
  software installed in it like apache nginx and also for the software to work the os is also
  installed like ubuntu server rhel or windows server for the websites we haev client side
  which is frontend and server side which is backend and that backend basically lets clients
  do the talking with the web server and database and vice versa and that backend is writtin
  in many languages like java python php c++ etc
- CIA triad confidentiality integrity availability confidentiality is the protection against
  unauthorized access integrity is the protection against unauthorized change and
  availability is making the resources or services available when needed whenever is system is
  to be secured the security engineer thinks in this way keeping the cia triad in mind what
  resources are to be protected from hacks and what resources and to be protected from change
  and what resources are needed to be up all the time and when a breach happens questions
  arise in this way what confidential information got stolen what information got changes and
  what resources went down 
- we have plain text that is human readable and then we have cipher text that is gibberish
  in crytography wat we do is convert the plain text in to cipher text their are two types of
  encryption symmetric encryption and asymmetric encryption in encryption we use key and an
  encryption algorithm to convert plain text into cipher text and then use key and
  decryption algorithm to convert a cipher text in to plain text in symmetric encryption we
  use a single key for encryption and decrytion but the key needs to be secure so that the
  attacker can not decrypt the message sent and also that key needs to be exchaged safely and
  for that we can not encrypt the key because then we have another key and teh same problem
  appears so for this asymmetric encryption came in which their are two keys one public key
  and private key one persons public key is used for encryption and that key is sent over the
  internet and teh same persons private key can only decrypt the cipher both these keys are
  mathematically linked in modern internet hybrid model of encryption is used asymmetric
  encryption is used for transfering the key between the two parties and then that same is
  used for symmetric encryption on both sides for faster cryptography and in this scenario
  one question arises what if the key sent over the internet that is the public key is sent
  from an attacker not a valid person so for mitigating this ca certifying autorities come
  in to play that gives certificates which show the public key as well as the owner of the
  key and the signature of that ca so that anyone can trust on it every os and browser has a
  certificate store which has certificates that are pre signed so that the process of
  verification or authentication becomes quick
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
  
