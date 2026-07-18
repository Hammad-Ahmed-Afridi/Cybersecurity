# Try Hack Me
## Security Engineer
- security engineer is a personnel that create secure systems and infrastructure deploy solutions for further security do audits and compliance and creates
  information security policies keeping security principles like cia trial authentication authorization access control non repudiation loggin and monitoring
  adn security frameworks like iso 27001 nist 800 soc 2 in mind including the governing laws and regulations like gdpr hippa pcidss a security engineer
  not only creates robust security posture of the entire organization but also maintain and improve it and make it resilient against the ever changing threat
  landscape he constantly do the checks and audits on the organization and its infrastructure and identifies the flaws and weaknesses and vulnerabilties in it
  and patches them and make the entire infra more robust keeping in view the organization goals and objectives in mind 
- symmetric encryption in which a single key is used for both the encryption and decryption and the algorithms used are aes advance encryption standard des
  data encryption standard blowfish 3des twofish idea international data encryption algorithm the security depends on the secrecy of the key one the key gets           compromised the whole communication gets compromised we can use openssl or gpg gnu privacy guard commands in the bash terminal for creating keys and also
  encrypting decrypting the cipher messages this is also called private key cryptography
- asymmetric encryption in which two keys are used public and private key and these keys are mathematically linked to each other but they can not be derived
  from each other the algorithms used are rsa rhimest shamir andleman dsa digital signature algorithm deffie hellman and this is also called public keycryptography
  in this the sender encrypts the message using the recipients public key which is available public and the recipient use his private key for decryption
  and we can use this for authenticity and non repudiation as well like if the sender wants to send something what is he does is encrypts the asset using his
  private key and sends it and the receiver uses the public key of the sender to decrypt it if the message is decrypted successfully the sender gets
  authenticated and the asset is also taken as real and legitimate and aslo teh sender can not deny that he did not send it hence eleminating non repudiation
  same tools can be used for this cryptography as well
- in modern times both these methods are used as a hybrid system we use asymmetric encryption for key exchange and then use sysmetric cryptography for actual
  communication becasue of how fast it is what happen is between two parties a single key is created by one person and for sending that key securily the sender
  encrypts it using the receipients public key and tehn sends it to receipient and than that person decrypts it using his private key in this way both of them get
  the key and then they can use the same key for encryption and decryption for secure communication but a question rise that is what if the attacker uses thepublic
  key of the receiver and encrypts his own key and then sends it to reciver and then that key is being used from that onwards so for this signatures and                certificates came in what happens is any piece of data is ecrypted using the senders private key in this case it is a symmetric key and this output can
  be taken as a signature now what happen is that the whole signature is then encrypted using the reciever public key and then sent to him and then that reciever
  then uses hsi private key to decrypt it and then uses the senders public key to decrypt the inner encryption and then the key is used becasue the inner               decryption would only be possible if and only if the actual person sent the key not any one else same happens in browsers using tls ssl certificates the              certificates are exchanegd to the browser from the server and the browser verifies using the its own private key for first decrytion and using the public key of      the server for the inner decryption and this key is present in the certificate store like hash is used and matched but i have just simplified it 
