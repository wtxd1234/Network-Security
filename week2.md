## Define encryption, decryption, plaintext, and ciphertext 
- __Encryption__ is the process of __transforming plaintext (readable data) into ciphertext (unreadable data)__ using a __secret key and an algorithm__.
- __Decryption__ is the reverse process of __recovering plaintext from ciphertext__ using the __same or a different key and algorithm__.
- __Plaintext__ is the __original message or data__ that is to be encrypted.
- __Ciphertext__ is the __encrypted message or data__ that results from the encryption process.

##  Symmetric vs asymmetric algorithms 
- __Symmetric algorithms__ use the __same key for both encryption and decryption__, while __asymmetric algorithms__ use __different keys for encryption and decryption__. The keys are mathematically related but not identical.

## What is the role of key/keys in symmetric and asymmetric algorithms? What is the relation between length of key and security?
- The role of key/keys in symmetric and asymmetric algorithms is to __provide security and confidentiality__ for the data.
- The __longer__ the key, the __more secure__ the algorithm, as it __increases the difficulty of brute-force attacks__. However, __longer keys also require more computational resources and time__ for encryption and decryption.

## Use Caesar Cipher with key 3 and encrypt the plaintext “attack at dawn” 
- Using Caesar Cipher with key 3 and __encrypting__ the plaintext "attack at dawn" results in the ciphertext __"dwwdfn dw gdzq"__.<br>![image](https://github.com/wtxd1234/Network-Security/assets/41671135/03cdb16f-9df6-4cc6-ad47-0c6450430989)


## Use Caesar Cipher with key 3 and decrypt the ciphertext “brute force attack”
- Using Caesar Cipher with key 3 and __decrypting__ the ciphertext "brute force attack" results in the plaintext __"yopqb cnbcp ylxbl"__. (Just reverse the table above)

## What is the size of key space in a Caesar cipher? 
- The size of key space in a Caesar cipher is __26__, as there are __26 possible shifts for the alphabet__.

## What’s the weakness of Caesar Cipher?
The weakness of Caesar Cipher is that it is __vulnerable to frequency analysis__, as the __relative frequencies of letters in the plaintext are preserved in the ciphertext__. Therefore, an attacker can __easily guess the key__ by __comparing the frequencies of letters in the ciphertext__ with those of a typical language.
