## Block cipher vs stream cipher 
- A __block cipher__ encrypts or decrypts a __fixed-length block__ of plaintext or ciphertext __at a time__, while a __stream cipher__ encrypts or decrypts a __continuous stream__ of plaintext or ciphertext __bit by bit__ or __byte by byte__.

## Main functions/operations of symmetric algorithms
- The main functions or operations of symmetric algorithms are __substitution__ and __permutation__.
- __Substitution__ replaces each plaintext element or group of elements __with a corresponding ciphertext element or group of elements__. 
- __Permutation__ changes the order of the elements in the plaintext or ciphertext __without altering their values__.

## Diffusion vs confusion 
- __Diffusion__ is a property that __hides the relationship between the plaintext and the ciphertext__ by spreading the influence of each plaintext bit over __many ciphertext bits__.
- __Confusion__ is a property that __hides the relationship between the ciphertext and the key__ by making the mapping between them complex and unpredictable.

## Function of S-BOX 
- An __S-BOX (substitution box)__ is a function that __maps a fixed number of input bits to a fixed number of output bits__, usually in a __non-linear way__. 
- It provides both __confusion and diffusion__ properties, contributing to the overall security of the cipher.

## Function of P-BOX 
- A __P-BOX (permutation box)__ is a function that __shuffles the bits of the input according to a predefined pattern__.
- It provides __diffusion__ by __spreading the output bits of one S-BOX across the inputs of several S-BOXes in the next round__.

## Relation between S-BOX and diffusion and confusion
- An __S-BOX__ provides both __diffusion and confusion__ by __changing the value and position of the input bits__ in a complex and __non-linear way__.
- The __output__ of an S-BOX depends on __the entire input and the key__, making it __hard to analyze or invert__.

## Relation between P-BOX and diffusion and confusion
- A __P-BOX__ provides __diffusion__ by __changing the position of the input bits, but not their values__.
- The __output__ of a P-BOX depends __only on the input, not the key__, making it __easy to invert__.
- However, a P-BOX indirectly contributes to confusion by __increasing the complexity of the S-BOXes in the next round__.

## Key size, block size, number of rounds of DES
- DES (Data Encryption Standard) uses a __56-bit key__, a __64-bit block__, and __16 rounds of encryption or decryption__.

## Operation of DES
1. DES operates on a __64-bit plaintext block__ by __dividing it into two 32-bit halves__, left and right.
2. Then, it applies __16 rounds of a Feistel cipher__ structure, where each round consists of __four__ steps: __expansion, key mixing, substitution__, and __permutation__.
3. In each round, the __right half__ is expanded from __32 bits to 48 bits__, __XORed with a 48-bit subkey__ derived from the main key, __passed through eight S-BOXes__ to produce a __32-bit output__, and __permuted by a P-BOX__.
4. The result is then __XORed with the left half__, and the __halves are swapped__.
5. After 16 rounds, the final swap is undone and the halves are concatenated to form the __64-bit ciphertext block__.
6. __Decryption is the same as encryption__, except that the __subkeys are used in reverse order__.
