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
