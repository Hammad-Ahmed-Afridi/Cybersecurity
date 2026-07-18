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
