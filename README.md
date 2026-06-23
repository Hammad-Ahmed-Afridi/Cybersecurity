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
  wide web tim berners lee
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
