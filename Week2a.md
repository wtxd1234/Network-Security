# Introduction to Cryptography
## Cryptography is Everywhere
- Secure Communications
- Encrypting files on the computer
- Data protection (DVD, Blu-ray...)
- Authentication, Digital Signature, Secret Sharing, E-Voting, E-Coin...

## Cryptography Goals
1. Confidentiality
2. Integrity
3. Non-repudiation
4. Authentication

## Cryptography Terminology
- __Plaintext__- original message
- __Ciphertext__- coded message
- __Cipher__- algorithm for transforming plaintext to ciphertext
- __Key__- info used in cipher known only to sender/receiver (must be private=unknown)
- __Encipher (encrypt)__- converting plaintext to ciphertext
- __Decipher (decrypt)__- recovering ciphertext from plaintext
- __Cryptography__- Study of encryption principles/methods
- __Cryptoanalysis (code breaking)__– Study of principles/methods of deciphering cipher text without knowing key
- __Cryptology__– Field of both cryptography and cryptoanalysis

![image](https://github.com/wtxd1234/Network-Security/assets/41671135/f0562da6-094b-4811-8519-914ad838dee0)

## Different Scenarios of Symmetric Cryptography
1. ___Single-Use Key (one-time key)___
   - Only used to encrypt a message
   - e.g. Each email is encrypted with a different key
2. ___Multi-Use Key (Many-time key)___
   - Used to encrypt multiple messages
   - The selection of “Algorithm” and “key” is critical in providing secure communication

## Symmetric Cryptography Mechanism
- 2 requirements for secure symmetric encryption:
  1. A strong encryption algorithm
  2. A secret key known only to sender/ receiver

## Encryption Scheme Security
- ___Unconditional security___
  - The cipher __can't be broken no matter how much computer power or time is available__ since the ciphertext provides insufficient information to uniquely determine the corresponding plaintext
- ___Computational security___
  - Cost of breaking the cipher > Value of the encrypted information
  - Time required to break the cipher > the useful lifetime of the information

## Cryptanalysis and Brute-Force Attack
- __Cryptanalysis__
  - Attack relies on the nature of the algorithm + some knowledge of the general characteristics of the plaintext
  - Attack exploits the characteristics of the algorithm to attempt to deduce a specific plaintext or to deduce the key being used
- __Brute-force attack__
  - Attacker tries every possible key on a piece of ciphertext until an intelligible translation into plaintext is obtained
  - On average, half of all possible keys must be tried to achieve success
