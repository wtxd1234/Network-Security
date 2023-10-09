# Introduction to cryptography
## Cryptography Algorithms
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/8c9a5b89-40d4-4069-a21b-c0b58068677e)

## Cryptography Systems
- Type of __encryption operations__ used:
   1. __Substitution__ (mapping to another character)
   2. __Transposition__ (rearranging the character)
- __Number of keys__ used:
   1. ___Single-key___: aka __Symmetric__, secret-key, private, or conventional cryptography 
(same key)
   2. ___Two-key___: aka __Asymmetric__, two-key, or public cryptography (different keys)
- Way in which __plaintext is processed__:
   1. __Block__ (only one block at a time)
   2. __Stream__ (process elements continuously)

## Classical Substitution Cipher
- A __substitution cipher__ replaces one symbol with another.
  - __Monoalphabetic__ replaces the same symbol with the same another symbol.
  - __Polyalphabetic__ replaces the same symbol with different symbols at each occurrence.

## Caesar Cipher
- It is one of the earliest and simplest methods of encryption.
- Used by Julius Caesar.
- It's a type of __substitution cipher__.
- Each letter of a given text is __replaced__ by a letter standing __three__ places further down the alphabet.
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/6d582990-a106-451a-b31a-0dccc7879477)

## Monoalphabetic Cipher
- Any letter can be substituted for any other letter (shuffle letters).
- Each letter has to have a unique substitute.
- Each plaintext letter maps to a different random ciphertext letter 
- The key space is 26! (greater than 4 ×10^26 possible keys)
- Now have a total of __26! keys__
- With so many keys, might think is secure 
- Brute Force approach would be too time consuming
- But would be !!!__WRONG__!!! 
- Statistical Analysis would make it feasible to crack the key
- Problem is language characteristics

## Cryptanalysis Monoalphabetic Cipher
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/e86afa61-4d13-4af6-85a4-e5a3cfa32ed0)
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/488a2ad3-dfcb-44c9-9a1d-508ce09fe586)

## Vigenère Cipher
- Developed by Blaise de Vigenere.
- Best known and simplest polyalphabetic substitution ciphers.
- In this scheme the set of related monoalphabetic substitution rules consists of the 26 Caesar ciphers with __shifts of 0 through 25__.
- To encrypt a message, a key is needed that is __as long as the message__ and usually, the key is a __repeating keyword__.
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/41871dfc-c9b5-4946-a58e-78dfc40a292f)

- __Encryption__: E<sub>i</sub> = (P<sub>i</sub> + K<sub>i</sub>) mod 26
- __Decryption__: D<sub>i</sub>= (E<sub>i</sub> - K<sub>i</sub>) mod 26
- Even this scheme is vulnerable to cryptanalysis, Because the key and the plaintext share the __same frequency__ distribution of letters, a __statistical technique__ can be applied.

## Transportation Ciphers
- It is a method of encryption that __scrambles the positions__ of characters without changing the characters themselves.
### Rail Fence Cipher
- Simplest transposition cipher.
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/41491033-387b-4407-b673-7ee346b3ab7f)

### Row Transposition Cipher
-  More complex transposition compared to Rail fence.
- Write the letters of the message out in __rows__ over a specified number of columns based on the __key length__.
- Then reorder the columns according to some key before reading off the rows.
- Any __spare spaces__ are filled with nulls, left blank, or placed by a character (example: X).
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/44bb63a4-d035-468a-9329-dc3d219fcad0)

## Cryptography is a precise mathematical science 
- Steps to Develop a Cryptographic Module/Algorithm:
1. Mathematically Modelling Threats
2. Developing an Algorithm to Address Threats
3. Proving Security through Mathematical Rigor
