# [Week 1](Week1.md)

- **Cybersecurity Subsets**: Focuses on information security, emphasizing the preservation of confidentiality, integrity, and availability of information, and network security, which protects networks from unwanted attacks and intrusions.

- **Security Key Principle/Objectives**:
  - **CIA Triad**: Confidentiality (preventing unauthorized access to data), Integrity (ensuring data is changed only in authorized ways), and Availability (ensuring data and systems are accessible to authorized users).
  - Additional Principles: Authenticity (verifying genuineness), and Accountability (tracking responsibilities).

- **Security Attacks**:
  - **Types**: Classified into passive (no system resource effect) and active attacks (alter system resources).
  - **Examples**: Passive attacks like message content release and traffic analysis; active attacks like masquerade, replay, message modification, and denial of service (DoS).

- **Security Services and Mechanisms**: Outlines various services (authentication, access control, confidentiality, integrity, nonrepudiation, availability) and mechanisms (cryptographic algorithms, data integrity, digital signature, etc.) in network security.

These are key concepts from Week 1, covering foundational principles of cybersecurity, types of security attacks, and the mechanisms and services used to counter these threats.

# [Week 2](Week2.md)

- **Introduction to Cryptography**: Explores the basic concepts and terminology of cryptography, including plaintext, ciphertext, cipher, key, encryption (encipher), and decryption (decipher).

- **Symmetric Cryptography Mechanisms**: Discusses the essentials of symmetric cryptography, emphasizing the importance of a strong encryption algorithm and a secret key known only to the sender/receiver.

- **Cryptography Systems**: Covers the types of encryption operations (substitution, transposition), number of keys used (single-key or symmetric, two-key or asymmetric), and how plaintext is processed (block or stream).

- **Classic Ciphers**: Examines historical ciphers such as the Caesar Cipher, Monoalphabetic Cipher, Rail Fence Cipher, and Row Transposition Cipher, including their methods and cryptanalysis.

This week provides an understanding of basic cryptographic concepts, symmetric cryptography mechanisms, various types of cryptography systems, and an introduction to classic ciphers.

# [Week 3](Week3.md)

- **Modern Cryptography and DES (Data Encryption Standard)**:
  - **Symmetric Cipher Types**: Focus on block ciphers, such as DES and AES, with an emphasis on block cipher processing.
  - **Feistel Cipher**: Explains the structure and functioning of Feistel ciphers, emphasizing their use of substitutions and permutations for secure encryption.
  - **Principles of Confusion and Diffusion**: Introduced by Claude Shannon, these principles are crucial for secure encryption.
  - **DES Features**: Detailed exploration of DES, including block size, key size, number of rounds, subkey generation, and the roles of S-boxes and P-boxes in the encryption process.
  - **DES vs. 3DES**: Comparison of DES with its more secure variant, 3DES, highlighting differences in key size, block size, number of rounds, and overall security strength.

This week covers advanced topics in modern cryptography, focusing on the structure and operation of block ciphers, especially DES and its variant 3DES.

# [Week 4](Week4.md)

- __AES__ is a __symmetric block cipher__ that operates on __128-bit blocks__ and supports key lengths of __128, 192, and 256 bits__.
- AES uses a __substitution-permutation network (SPN)__ structure, which consists of __four__ stages: __SubBytes, ShiftRows, MixColumns__, and __AddRoundKey__.
- AES has __10, 12, or 14 rounds__, depending on the __key length__. Each round uses a subkey derived from the main key using a key expansion algorithm.
- AES is __fast, simple, and resistant to known attacks__.

# [Week 5](Week5.md)

- __RC4__ is a __symmetric stream cipher__ that __encrypts one byte at a time using a pseudorandom keystream__.
- RC4 has __two__ steps: __key scheduling algorithm (KSA)__ and __pseudorandom generation algorithm (PRGA)__.
- KSA __initializes a 256-byte state vector S__ using a __variable-length key__.
- PRGA __generates the keystream__ by __permuting__ and __swapping the elements of S__.
- RC4 is __fast and easy to implement__, but has several vulnerabilities and weaknesses.

# [Week 6](Week6.md)

- __Hash functions__ are __one-way functions__ that __map an arbitrary-length input to a fixed-length output__, called a __hash__ or a __digest__.
- Hash functions are used for various purposes, such as __message authentication, digital signatures, password storage__, and __pseudorandom number generation__.
- Hash functions must satisfy __three__ properties: __preimage resistance, second preimage resistance__, and __collision resistance__.
- __Secure Hash Algorithm (SHA)__ is a family of hash functions __developed by NIST__, which includes SHA-1, SHA-2, and SHA-3. SHA algorithms have different output sizes and security levels.

Here are some detailed notes for week 7 and week 8 from the pdf provided:

# [Week 7](Week7.md)
- **Asymmetric Encryption**: A type of encryption that uses a pair of mathematically related keys: a public key and a private key. The public key can be used to encrypt messages or verify signatures, while the private key can be used to decrypt messages or sign messages.
- **Principles of Public-Key Cryptosystems**: The public key is widely distributed and known to everyone, while the private key is kept secret by the owner. The public key and the private key are linked by a one-way function that is easy to compute in one direction but hard to invert.
- **Public-Key Cryptosystems**: Some examples of public-key cryptosystems are RSA, Diffie-Hellman, ElGamal, and Elliptic Curve Cryptography. They are based on different mathematical problems, such as factoring large numbers, discrete logarithms, or elliptic curve operations.
- **Applications for Public-Key Cryptosystems**: Public-key cryptosystems can be used for encryption/decryption, digital signature, key exchange, and other purposes. They provide security services such as confidentiality, integrity, authentication, and non-repudiation.
- **Requirements for Public-Key Cryptography**: The public-key algorithms must be computationally secure, meaning that there is no efficient algorithm to break them. The key sizes must be large enough to resist brute-force attacks. The algorithms must also be efficient and practical to implement and use.
- **Diffie-Hellman Algorithm & Key Exchange**: A key agreement protocol that allows two parties to securely exchange a secret key over a public channel. It is based on the concept of modular arithmetic and discrete logarithms. It is vulnerable to man-in-the-middle attacks if the public keys are not authenticated.
- **RSA Algorithm**: A public-key cryptosystem that can be used for both encryption/decryption and digital signature. It is based on the difficulty of factoring large numbers. It involves choosing two large prime numbers, computing their product and Euler's phi function, selecting an encryption key and its inverse, and performing modular exponentiation.

# [Week 8](Week8.md)
- **Key Distribution and Management**: The process of creating, protecting, storing, exchanging, replacing, and using cryptographic keys for a cryptographic system. It involves addressing the challenges of key sharing, key obtaining, key changing, and key restricting.
- **Symmetric Key Distribution using Symmetric Encryption**: A method of distributing secret keys using a symmetric encryption algorithm, such as AES or DES. It requires a trusted third party, such as a key distribution center (KDC), to generate and distribute session keys to the communicating parties. It also requires a secure way to share the master keys between the parties and the KDC.
- **Symmetric Key Distribution using Asymmetric Encryption**: A method of distributing secret keys using an asymmetric encryption algorithm, such as RSA or Diffie-Hellman. It does not require a trusted third party, but it requires the parties to have each other's public keys. It can provide both confidentiality and authentication in the exchange of secret keys.
- **Distribution of Public Keys**: A method of distributing public keys using a public key infrastructure (PKI), which is a system of certificates, certificate authorities (CAs), and other entities that verify and manage the public keys. A certificate is a digital document that binds a public key to an identity, and it is signed by a CA. A certificate can be used for secure communication, encryption, or authentication purposes.
- **Digital Certificates**: A type of public key certificate that follows a standard format, such as X.509. It contains information about the owner of the key, the issuing CA, the validity period, the signature algorithm, and the digital signature of the CA. It can be verified by checking the signature of the CA and the validity of the certificate.

# [Week 10](Week10.md)
- **Transport Level Security**: SSL and TLS are protocols that provide security services to application layer protocols using TCP. They consist of multiple subprotocols: record, handshake, change cipher, and alert. They provide confidentiality, integrity, and authentication for web and other Internet applications.
- **HTTPS**: HTTPS is HTTP over SSL or TLS. It uses port 443 and encrypts the URL, contents, forms, cookies, and header of the web requests and responses. It also authenticates the server using a certificate.
- **Firewall**: A firewall is a network security device that prevents unauthorized access to a network. It inspects incoming and outgoing traffic using a set of security rules to identify and block threats. Firewalls can be network-based or host-based, and can operate on different layers of the network stack. Firewalls can be physical hardware, digital software, SaaS, or virtual private cloud.
