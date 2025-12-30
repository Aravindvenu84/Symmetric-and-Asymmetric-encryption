# Symmetric-and-Asymmetric-encryption

Symmetric and Asymmetric Encryption
Introduction

Encryption is a core concept in cybersecurity used to protect sensitive information from unauthorized access. It converts readable data (plaintext) into an unreadable format (ciphertext) using cryptographic algorithms and keys. Based on how keys are used, encryption is broadly classified into symmetric encryption and asymmetric encryption.

a. Main Categories of Encryption
1. Symmetric Encryption

Symmetric encryption uses a single secret key for both encryption and decryption. The same key must be securely shared between the sender and the receiver before communication begins.

2. Asymmetric Encryption

Asymmetric encryption uses two different but mathematically related keys:

Public Key – shared openly

Private Key – kept secret by the owner

Data encrypted with one key can only be decrypted using the other.

b. Encryption and Decryption Process
Symmetric Encryption Process
Sender                           Receiver
  |                                 |
  |-- Plaintext ------------------> |
  |-- Encrypt using Secret Key ---->|
  |                                 |
  |-- Ciphertext -----------------> |
  |                                 |
  |<-- Decrypt using Same Key ------|
  |                                 |
  |-- Original Plaintext ---------> |


Key Points:

Same key is used for encryption and decryption

Fast and efficient

Secure key distribution is challenging

Asymmetric Encryption Process
Sender                              Receiver
  |                                    |
  |-- Plaintext ---------------------> |
  |-- Encrypt using Receiver's Public Key
  |                                    |
  |-- Ciphertext --------------------> |
  |                                    |
  |<-- Decrypt using Private Key ----- |
  |                                    |
  |-- Original Plaintext ------------> |


Key Points:

Uses public and private key pair

Eliminates key-sharing risks

Slower compared to symmetric encryption

c. Advantages, Limitations, and Applications
Comparison Table
Aspect	Symmetric Encryption	Asymmetric Encryption
Keys Used	Single shared key	Public and private key pair
Speed	Very fast	Slower
Security Level	High (if key is protected)	Very high
Key Distribution	Difficult and risky	Secure and scalable
Scalability	Poor for large networks	Good for large systems
Algorithms	AES, DES, Blowfish	RSA, ECC, DSA
Common Applications	Disk encryption, VPNs, database security	SSL/TLS, digital signatures, secure key exchange
d. Hybrid Encryption (Real-World Implementation)

In real-world systems, symmetric and asymmetric encryption are used together to combine performance and security.

Example: HTTPS (SSL/TLS)
Client                       Server
  |                             |
  |-- Request Public Key -----> |
  |-- Encrypted Session Key --> |
  |                             |
  |== Secure Symmetric Communication ==


Explanation:

Asymmetric encryption securely exchanges a symmetric session key

Symmetric encryption is then used for fast data transfer

Conclusion

Symmetric and asymmetric encryption serve different but complementary purposes in cybersecurity. Symmetric encryption is efficient and fast, while asymmetric encryption provides secure key exchange and authentication. Modern secure systems rely on hybrid encryption to ensure confidentiality, integrity, and trust in digital communications.
