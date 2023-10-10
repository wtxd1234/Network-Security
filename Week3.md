# Modern Cryptography and DES
## Types of Symmetric Cipher
- Way in which __plaintext is processed__ (recap):
  - __Block__ (only one block at a time)
  - __Stream__ (process elements continuously)
- Many current ciphers are block ciphers (a broader range of apps)
- Focus on __DES__ (Data Encryption Standard) and __AES__ (Advanced encryption standard)

## Stream Cipher & Block Cipher
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/9d18b3bd-d5e4-481b-adf3-94c48b9d7f7c)

### Block Cipher
- Usage: 
  - ___File Transferring___: When transferring files over a network or the internet, it is crucial to protect the content from unauthorized access.
  - ___Email___: Email communications often contain sensitive or confidential information, and encrypting the email content is essential to maintain privacy. Pretty Good Privacy __(PGP)__ or Secure/Multipurpose Internet Mail Extensions __(S/MIME)__.
  - ___Databases___: Encryption of the database content provides an additional layer of security. Block ciphers can be used to encrypt the database files or individual columns within a database.
- If the message is not a multiple of n bits, then what do we do?
  - __Padding__
    - If the size is __less__ than n bits, then it will pad it by 0s and make it n bits.
    - if it is __greater__ than n bits but not a multiple of n, then divide them into n bit blocks, and the last block, which is left, is obviously less than n bits; in that case, it also pads the last block and makes it equal to n bits.
### Block Cipher Example
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/e0bef589-808d-4e61-9f62-394fc8c46dc9)

## Modes of Operation
- In __block cipher cryptography__, the mode of operation refers to the __method used to encrypt__ plaintext data in blocks of fixed size.
- The real data contains lot of __redundancy__. If the data is encrypted using the normal Block cipher the redundancy __might be reflected in ciphertext__ as well. This gives attacker __useful information__ to perform __statistical/pattern__ analysis and find the key.

### Most Common Modes of Operation
1. ___Electronic Codebook (ECB)___: Each block of plaintext is encrypted separately and independently. This mode is simple but not very secure, as identical __plaintext blocks will result in identical ciphertext blocks__.
2. ___Cipher Block Chaining (CBC)___: Each plaintext block is XORed with the previous ciphertext block before encryption. This adds an extra layer of security and __prevents identical plaintext blocks from producing identical ciphertext blocks__.
3. ___Counter mode (CTR)___: The block cipher is used to generate a keystream, which is
XORed with the plaintext to produce the ciphertext. __This mode allows for parallel
encryption and decryption, and is often used in high-speed communication
networks__.
4. ___Galois/Counter Mode (GCM)___: This mode combines the Counter mode with a Galois field multiplication to provide both confidentiality and integrity protection. It is widely used in modern protocols such as __TLS and IPsec__.
5. ___Output Feedback (OFB)___: In OFB mode, the block cipher is used to generate a __keystream of pseudo-random bits__ that is XORed with the plaintext to produce the ciphertext.
6. ___Cipher Feedback (CFB)___: This mode uses the block cipher to encrypt the previous ciphertext  block, which is then XORed with the plaintext to produce the ciphertext. Like CBC, __it provides some randomness__ to the encryption process, but it is also a self-synchronizing stream cipher.

## Motivation for Feistel Cipher
- A block cipher operates on a plaintext block of n bits to produce a 
ciphertext block of n bits
- There are 2^n possible different plaintext blocks
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/a64703d9-3905-42ab-a8ee-342b012e0f6d)
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/72219ffd-ec91-4d09-9304-baa6e77f2cb5)

## Feistel Cipher
- ___Feistel cipher___: A symmetric encryption algorithm that uses a structure __composed of multiple rounds__ to process a plaintext message into a ciphertext message. It use of a cipher that alternates __substitutions and permutations__.
  - ___Substitutions___: Each plaintext element or group of elements is uniquely replaced by a corresponding ciphertext element or group of elements.
  - ___Permutation___: No elements are added or deleted or replaced in the  sequence, rather the order in which the elements appear in the sequence is changed.
- They are used to provide:
  - ___Diffusion___: The diffusion is a property, which __hides__ the relationship between the __ciphertext and the plaintext__ to the attacker.
  - ___Confusion___: the property, which __hides__ the relationship between the __ciphertext and the value of the key__.
- A proposal by __Claude Shannon__ to develop a product cipher that
alternates confusion and diffusion functions (used by many
significant symmetric block ciphers)
