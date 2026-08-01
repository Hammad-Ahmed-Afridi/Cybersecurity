# Try Hack Me
## Security Engineer
- A security engineer is a professional who creates secure systems and infrastructure, deploys solutions for further security, performs audits and
  compliance checks, and creates information security policies. They keep security principles like the CIA triad, authentication, authorization, access
  control, non-repudiation, logging, and monitoring in mind, as well as security frameworks like ISO 27001, NIST 800, and SOC 2, including governing laws
  and regulations like GDPR, HIPAA, and PCI DSS. A security engineer not only creates a robust security posture for the entire organization but also
  maintains, improves, and makes it resilient against the ever-changing threat landscape. He constantly runs checks and audits on the organization and
  its infrastructure, identifies flaws, weaknesses, and vulnerabilities, and patches them to make the entire infrastructure more robust, while keeping
  the organization's goals and objectives in mind.
- Symmetric encryption is a method in which a single key is used for both encryption and decryption. The algorithms used are AES (Advanced Encryption
  Standard), DES (Data Encryption Standard), Blowfish, 3DES, Twofish, and IDEA (International Data Encryption Algorithm). The security depends entirely
  on the secrecy of the key; once the key gets compromised, the whole communication gets compromised. We can use OpenSSL or GPG (GNU Privacy Guard)
  commands in the bash terminal for creating keys and also encrypting and decrypting cipher messages. This is also called private-key cryptography.
- Asymmetric encryption is a method in which two keys are used: a public and a private key. These keys are mathematically linked to each other, but they
  cannot be derived from one another. The algorithms used are RSA (Rivest-Shamir-Adleman), DSA (Digital Signature Algorithm), and Diffie-Hellman. This is
  also called public-key cryptography. In this system, the sender encrypts the message using the recipient's public key (which is available publicly), and
  the recipient uses his private key for decryption. We can use this for authenticity and non-repudiation as well. For example, if the sender wants to
  send something, what he does is encrypt the asset using his private key and send it. The receiver then uses the public key of the sender to decrypt it. If
  the message decrypts successfully, the sender gets authenticated, the asset is taken as real and legitimate, and the sender cannot deny sending it,
  hence establishing non-repudiation. The same tools can be used for this type of cryptography as well.
- In modern times, both these methods are used together as a hybrid system. We use asymmetric encryption for key exchange and then use symmetric cryptography
  for the actual communication because of how fast it is. What happens is that between two parties, a single key is created by one person. To send that key
  securely, the sender encrypts it using the recipient's public key and sends it. The recipient then decrypts it using his private key. In this way, both of
  them get the key, and they can then use that same key for encryption and decryption to maintain secure communication.
- But a question arises: what if an attacker uses the public key of the receiver, encrypts his own key, sends it to the receiver, and that malicious key is
  used from that point onwards? To solve this, signatures and certificates came in. What happens is that a piece of data (in this case, the symmetric key)
  is encrypted using the sender's private key, and this output is taken as a digital signature. Then, the whole signature is encrypted using the receiver's
  public key and sent to him. The receiver uses his private key to decrypt the outer layer, and then uses the sender's public key to decrypt the inner
  encryption. The key is only used after this because the inner decryption would be possible if and only if the actual person sent the key, not anyone else.
  The same thing happens in browsers using TLS/SSL certificates. The certificates are exchanged from the server to the browser, and the browser verifies them.
  It uses its own private key for the first decryption, and uses the public key of the server for the inner decryption. This key is validated against
  the certificate store where a hash is used and matched—though I have just simplified it here.
- idm identity manaagement is the managemnet of identities their creation their storage their managemnet and their deletion for example a user comes and is
  given his own card which includes name email contact number and address then we have iam identity and access managemnet which manages the access of the
  user or the identity within the entire system based on authentication authorization accountabillity non repudiation and logging and monitoring for example
  the user created has following access and when he shows his card he can access certain assets and locations idm comes under iam 
- access control models include discretionary access control in which the owner of the asset or a file can allow or deny further user activity on that particular
  asset or file role based access control in which specific groupd are created which role groups and taht entire group is given access to certain asset and
  users are added to it and those users would automatically get the permissions and if they are removed from the group they will not have them and then we have
  mandatory access control in which assess is given based on clearance levels like bottom clearance can not access top clearance level assets and lastlly we have
  attributre based access control in which assess in given on the basis of attributes 
- in an entire infrature their are several services and systems that are used by people for different type of work and they have to access them regulary for
  work but they can not put in identity and password every time accesing the services so sso comes in play single sign on which means that the user gets
  authenticated once and can use evrey service authorized to him for that specific session without further authentiations 
- governance is basically creating goals and policies and best practices of an organization and compliance is basically checking if the organization
  is following the industry standards and protocols in its activities and procedures and systems grc governance risk and compliance is the creating policies
  procedures for and organization succcess and making these policies in accordance with the regualtions and frameworks and steps taken to
  increase the security of an org by defining the scope and systems checking for implemented controls reviewing them doing risk assessment finding
  vulnerabilties if any recommending best security practices also these practices should be in accordance with the industry frameworks like iso 27001
  and soc 2 and legal regulatiosn like gdpr pcidss hippa recommend practices to implement these recommendations and then reviewing the adoption and
  constantly updating the information security policy for making the entire organization more robust against the ever changing threat landscape
- in grc the risk managemnet is the core part and invloves the identification of all the systems and resources in an organization reviewing them against
  known threats and attacks find vulnerabilties develop security for those systems and resources implement them ad review and audit the implementation adoption
  and constantly update the policy against the changing threat landscape in this we haev multiple frameworks which comes down to the core principle mentioned
  above the risk assessment focuses on vulnerabilities related to auithentication authorization access cotrol non repudiation denial of service privilage
  escalation compromsing confidentiality integrity and availabilty so in risk assesment the attacks against the vulnerabilities are first found and then their
  impact is kept in view and then prioritize them and do patches and fixes in this assessment we use MITRE ATTACK attacker tactics techniques and common
  knowledge is a frame work or a database of all the attacks that happened and hwothey happened and what tacktic were used by the attacker and what vulnerabilties
  they exploited we also use and we can use them to get knowledge against our systems and we use the tool called attack navigator for searching and finding
  when the assessment is done the vulnerabilties are found against the system teh attack paterns are also found then steps are taken to mitigate these risks by
  either patching them accepting them if the patching is far expensive then the loss or risk transfer and also before this process risk analysis is done
  in which risk is prioritized on the basis of its impact and damage and the probability of happening and then they are cared for and we find vulnerabilties in
  the system using gui tools like nessus openvas and get to know the vulnerabilties against the known cve database and then also use these vulnerabilties
  to find the attack patterns used by attackers using mitre attack framework and also use this knowledge to patch them and also implement controls if patching
  them is costly
- while a network is being established in an organization certain aspects are kept in mind like segmentation zone pair using secure protocols etc we can
  segemnt a network using vlan technology this happens at layer 2 switch and we can either use two or more switches or be resouce consious and use a single
  switch a single switch will not make the seperate networks one network instead for them to communicate we either remove the layer 2 switch and use a layer 3
  switch or use a router with the layer 2 switch this helps in access control like if in a network attackers intruded and got control we can apply certain
  rules and policies that will block them from lateral movement in a network ad privilage escaltion zone pair is implimenting rules and policies so that traffic
  route could be in one direction not both or between the specific network zones we also have a dmz demilitarized zone that acts as a border between the internal
  org network and external internet we can implement firewalls ids ips at specifc locations inside a network or at the start of the vlans so that the traffic
  could be monitored and controlled 
- linux device hardening include linux server or linux os hardware hardening we can accomplish this by using strong passwords and also enabling a strong
  password policy also increasing the physical security by adding a boot password which will ask you for a password before the boot and it can not be changed by
  a hacker like a normal log in password can be changed when physically present hardening the software and hardware ports that are not used and also
  disabing services and packages that are not required implementing strict access control so thta even if the attacker got access to an account on the system
  he can not do privilage escalation to a root user updating and upgrading the system to the newest releases and logging the events and monitoring them
  continuously for any failures or malicios activities also disable direct root login over ssh we can also use firewall like ufw uncomplicated firewall that will
  also allow or disallow packets connection to the linux device and for data stored we should use the encryption and use the strongest encryption algorithm and
  secure the keys and also use the encryption for data in transit between the systems and backup neccessary data as well
- windows device hardening can be achieved as the same as that of linux like we can implement strong iam policies like password strength principle of least
  privilage and other use firewall for monitoring traffic and allowing and blocking it use a boot loader password for uefi/bios harden the unused software and
  hardware ports remove the unneccessary services and download apps and softwares from trusted sources disable rdp login to administrator account and logging
  and monitoring the events in the windows event viewer use bitlocker encryption for data encryption use ssecure browsing 
- for active directory hardening and network device hardening we use some of the above steps for them as well
- for managing systems or devices on a network like servers firewall ips ids routers switches we can use cli as well as gui applications
- we have network protocols that became insecure because the data sent over the internet using these protocols was not encrypted so ssl tls was used to wrap
  these protocols for data encryption at application layer we have http dns ftp smtp pop3 imap telnet which became https dnssec ftps smtps pop3s imaps and ssh
- at network layer we have ipsec which came after ppp and pptp protocol which is used by vpn for secure encrypted communication over the internet also we have
  icmp for pinging devices over the network arp protocol
- virtializations is a process through which we create muktiple software based infrastructure like computers with their own cpu ram storage while utilizing a
  single host infra so that we can maximize the resource usage and reduce costs take for example we have a server if we run only one os on it we will be
  wasting up so much resources so what we do is create virtual environmnets each seperate and isolated from each other having their own resouces we can
  accomplish virtualization using a software called hypervisor it sits between the host and the virtual environments and allow the virtaul environment to
  communicate with the host and share resources we have two types of hypervisors tyep 1 which sits directly on top of the server or machine and create vms
  and type 2 which sits on top of the host os that is on the server like first we haev server than the server os than the hypervisor running on that os
  and then that hypervisor creating multiple vms on top of host os type 1 example is vmware ex and type 2 is vmware workstation and oracle virtualbox virtual
  machines are compute engines having their own cpu ram storage resources we use them for secure testing of software in isolated environemnts or for actually
  using them for other purposes in clud computing
- in correspondence to vms and hypervisor and virtualization we have containers containers are softwares solutions that package the code its dependencies
  in to a single container and allow them to run anywhere we sue containers beccause it is less resource consuming than vms like we can run them on host os
  without needing any extra compute or storage and we can set up containers using docker first we use docker to create a docker file than create a docker
  image and then create a docker container and run it and in order to manage multiple docker containers we use kubernetes it is a orchestration software
  that hepls in managing docker containers like creating new copies when needed and deeting them when not required 
- cloud computing is getting compute storage network resources without owning the actual hardware on pay as you go pricing model the cloud service providor
  sets up the hardware and the consumer gets to bu the services we have three cloud computing models like iaas paas saas in infrastructure as a service the
  sloud providor sets up the entire infra and you have to manage the internals like os installed apps running like they set up the servers do teh external
  networking and provide power and the rets is managed by the consumer in platforms as a service included services include the ones in the iaas and os
  as well and you just ahve to manage the code and application on it and is softwware as a service everything is included includig the app and code and you
  on consumer side just use the app for bsusiness or personnel purposes we use cloud computing for a numebr of resons like getting compute storage
  processing power without actually owning the hardware get robust security provided by cloud provider get backups for business continuity and disaster
  recovery 
- cloud deployment models include public cloud private cloud hybrid cloud and community cloud in public cloud we have services assessble to everyone like
  apart from us cloud provider can set up other users on a single server using that server resources using virtualization for isolation and in private
  cloud cloud providor set up private set ups dedicated for a single user and then we have hybrid cloud which compose of public private and on prmise it
  infra and then we have community cloud which is for users that require same services or resources or configurations from the cloud providor so cloud
  providor set it up once and then copy them for all the users in a community
- cloud security is security cloud encironment both physically and software point of view as well physical security is managed by the service provider and in
  some cloud computing models like saas the software security is also managed by them but in cloud the infra when given to the consumer has to be software wise
  managed by the consumer in cloud security their are many things to take care of like when data is stored encryption at rest should be used using strong industry
  recognized algos when in transit same algos should be used and when destroying data specifci steps like encrypting the data and the destroying the keys and then
  data when using the data secure connections should be estaleshed and aslo in cloud infra proper virtual environements should be set up for maximum isolation
  implementing strict iam policies and rules and least access control and to overcome privilage escallation and lateral movement implemeting firewalls to cloud
  instances inplementing access control lists logigng and monitoring events for malicios and improper behavior in cloud computing the security is shared
  and is maintained by both the services provider and service consumer and this is called shared responsiblity model 
- owasp api security includes bola which stands for broken object level authorization it is like idor in which a simple input can cause unauthorized access to
  resources that do not have to be given access to we have bua broken user authentication that can be exploited to get authenticated without proper credentials
  or identity or account we have excessive data exposure in which when api calls or api request are made to a server or database the server or db response
  exposes too much data that is not required or is confedential we have no rate limiting and because of which too many api requests could be made exhausting
  the resources or denial of service happens we have security misconfigurations like using basic or default credentials ro not setting up apis properly
  we have injection attacks like code injection sql injection we have no proper logging and monitoring in which the usage of api their request and response is
  not properly logged and monitored and hacker can take advantage of it by remaining invinsible 
- sdlc software developemnt lifecycle is basically procedures and steps invloved in software development from planning to designing to coding to building to
  testing to releasing to deploying to monitoring and then this becomes a loop and is infinite sdlc is performed using a framework or methodoogy called devops
  development and operation it is teh integration and colabration of many teams working on a project in a synchronous way and each one team doing their work
  and pushing and testing it through automatic ci/cd continuous integration continuous development pipelines for maximum productivity and speed and time to
  market we have ssdl which is basically adding security in sdlc process like devops becomes devsecops previously security was implemented at the end which
  led to many issues like cost time consumptions and many vulnerabilities to be solved and a need for shifting left strategy was felt like moving to the left
  which is the beginning of the sdlc process for maximum security and to overcome other issues as well
- we have multiple tools that are being used in devsecops are they are categorized into SAST DAST IAST RASP tools SAST stands for static application security
  testing it is a white box testing method which means that the code is being scanned and reviewed for finding vulnerabilities we have manual and automated
  scans and reviews and analysis DAST stands for dyanamic application security testing it is a black box method in which no code base is provided and the
  tool or manual person do the testing an dfind vulnerabilities just like a real attacker we use tools like burpsuite or owasp zap IAST interactive application
  security testing is a method in which the code is also available and also a real attacker scenario is also created for finding vulnerabilties easily and
  which greater accuracy RASP runtime appliation self protection is a method in which tools are deployed on teh application server so that it can monitor the
  traffic or unwanted behaviour and mitigate them and provide robust security  
- IR incident response and IM incident management are processes which are carried out at the start and during and after the attack incident response is done
  when the attack or incident happens and we detect it respond to it and take appropriate actions and also take the the organizational appraoch as well
  apart from technical approaches is process that is carried out which includes conatining the attack and eradicating it both the IR and IM are not seperate
  processes combined as one we have four levels of incidents that ae managed by four levels of team first level is managed by soc team which is
  basic incident the next level is computer emergency readiness team level which is level 2 incidet responders and
  then the next level is computer security incident response team which are level three incident responders and then finally we have crisis managemnet team for
  level 4 which can take nuclear actions like shutting the whoe system down if the compromise is large scale and gotten a strong hold whe ever incident happens
  following steps are taken before the incident preperation and protection is done then during incident detect respond contain eradicate and recovery and after
  the recovery post incident recovery is done which include many processes and aslo includes lessons learned 
- whenerv incident happens it is not a good protocol to turn of the systems becasue it can cause business disruption and lawsuites and more importantly the
  system volatile memory has so much information regarding the attack or incident that it can be used in forensics but it gets lost so when the incident
  happens and we detect it we dont shut the system down what we do is as we are trained in table top excercise we use playbooks for actiosn like we isolate
  the affected system we inform the relevant stakeholders we keep the systems running we document our actions during attack 
- Governance, Risk, and Compliance (GRC) is a continuous, cyclical methodology designed to protect an organization by establishing and maintaining an Information
  Security Management System (ISMS) aligned with international standards and regulations such as ISO/IEC 27001, NIST SP 800-series, GDPR, and PCI DSS. The process
  begins by defining the scope—identifying the specific systems, people, and organizational governance structures required to support long-term business growth—
  before moving into risk management. In this phase, assets within the scope are analyzed to determine the probability and impact of potential threats, resulting in
  a severity rating (critical, high, medium, low). These theoretical risks are then validated through actual security assessments, such as vulnerability scanning
  and penetration testing, and addressed through clear risk decisions: mitigating them using technical playbooks and tabletop exercises, accepting them within
  defined tolerance levels, transferring them via insurance, or avoiding them entirely. Crucially, every single measure, process, and decision must be
  thoroughly documented because internal, third-party, and certifying auditors rely strictly on this evidentiary trail to verify compliance, grant the Authorization
  to Operate (ATO), and build customer trust. Ultimately, compliance is not a one-time certification milestone but an ongoing process of continuous improvement
  that adapts to an ever-changing threat landscape.
- ISO 27001 is the only standard in the family against which an organization can get officially certified, while ISO 27000 serves as the vocabulary glossary and
  ISO 27002 functions as the detailed instruction playbook
