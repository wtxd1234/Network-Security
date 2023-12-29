## Block cipher vs stream cipher 
- A __block cipher__ encrypts or decrypts a __fixed-length block__ of plaintext or ciphertext __at a time__, while a __stream cipher__ encrypts or decrypts a __continuous stream__ of plaintext or ciphertext __bit by bit__ or __byte by byte__.

## Main functions/operations of symmetric algorithms
- The main functions or operations of symmetric algorithms are __substitution__ and __permutation__.
- Substitution replaces each plaintext element or group of elements with a corresponding ciphertext element or group of elements. Permutation changes the order of the elements in the plaintext or ciphertext without altering their values.

## Diffusion vs confusion 
Diffusion is a property that hides the relationship between the plaintext and the ciphertext by spreading the influence of each plaintext bit over many ciphertext bits. Confusion is a property that hides the relationship between the ciphertext and the key by making the mapping between them complex and unpredictable.

##Function of S-BOX 
An S-BOX (substitution box) is a function that maps a fixed number of input bits to a fixed number of output bits, usually in a non-linear way. It provides both confusion and diffusion properties, contributing to the overall security of the cipher.

## Function of P-BOX 
A P-BOX (permutation box) is a function that shuffles the bits of the input according to a predefined pattern. It provides diffusion by spreading the output bits of one S-BOX across the inputs of several S-BOXes in the next round.

## Relation between S-BOX and diffusion and confusion
An S-BOX provides both diffusion and confusion by changing the value and position of the input bits in a complex and non-linear way. The output of an S-BOX depends on the entire input and the key, making it hard to analyze or invert.

## Relation between P-BOX and diffusion and confusion
A P-BOX provides diffusion by changing the position of the input bits, but not their values. The output of a P-BOX depends only on the input, not the key, making it easy to invert. However, a P-BOX indirectly contributes to confusion by increasing the complexity of the S-BOXes in the next round.

## Key size, block size, number of rounds of DES
DES (Data Encryption Standard) uses a 56-bit key, a 64-bit block, and 16 rounds of encryption or decryption.

## Operation of DES
DES operates on a 64-bit plaintext block by dividing it into two 32-bit halves, left and right. Then, it applies 16 rounds of a Feistel cipher structure, where each round consists of four steps: expansion, key mixing, substitution, and permutation. In each round, the right half is expanded from 32 bits to 48 bits, XORed with a 48-bit subkey derived from the main key, passed through eight S-BOXes to produce a 32-bit output, and permuted by a P-BOX. The result is then XORed with the left half, and the halves are swapped. After 16 rounds, the final swap is undone and the halves are concatenated to form the 64-bit ciphertext block. Decryption is the same as encryption, except that the subkeys are used in reverse order.
