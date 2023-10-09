# Modern Cryptography and DES
## Types of Symmetric Cipher
- Way in which __plaintext is processed__ (recap):
  - __Block__ (only one block at a time)
  - __Stream__ (process elements continuously)
- Many current ciphers are block ciphers (a broader range of apps)
- Focus on __DES__ (Data Encryption Standard) and __AES__ (Advanced encryption standard)

## Stream Cipher & Block Cipher
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/9d18b3bd-d5e4-481b-adf3-94c48b9d7f7c)

## Block Cipher
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
