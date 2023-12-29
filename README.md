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

# Week 4

- AES is a symmetric block cipher that operates on 128-bit blocks and supports key lengths of 128, 192, and 256 bits.
- AES uses a substitution-permutation network (SPN) structure, which consists of four stages: SubBytes, ShiftRows, MixColumns, and AddRoundKey.
- AES has 10, 12, or 14 rounds, depending on the key length. Each round uses a subkey derived from the main key using a key expansion algorithm.
- AES is fast, simple, and resistant to known attacks.

# Week 5

- RC4 is a symmetric stream cipher that encrypts one byte at a time using a pseudorandom keystream.
- RC4 has two steps: key scheduling algorithm (KSA) and pseudorandom generation algorithm (PRGA).
- KSA initializes a 256-byte state vector S using a variable-length key.
- PRGA generates the keystream by permuting and swapping the elements of S.
- RC4 is fast and easy to implement, but has several vulnerabilities and weaknesses.

# Week 6

- Hash functions are one-way functions that map an arbitrary-length input to a fixed-length output, called a hash or a digest.
- Hash functions are used for various purposes, such as message authentication, digital signatures, password storage, and pseudorandom number generation.
- Hash functions must satisfy three properties: preimage resistance, second preimage resistance, and collision resistance.
- Secure Hash Algorithm (SHA) is a family of hash functions developed by NIST, which includes SHA-1, SHA-2, and SHA-3. SHA algorithms have different output sizes and security levels.
