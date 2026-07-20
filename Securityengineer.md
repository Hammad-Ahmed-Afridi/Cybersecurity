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
