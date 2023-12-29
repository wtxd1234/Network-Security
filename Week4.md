## Avalanche effect
This is the property that a small change in the plaintext or the key result in a significant change in the ciphertext. It contributes to enhance security by making it harder for attackers to use cryptanalysis methods to uncover the original plaintext or key, as they cannot predict how the ciphertext will change based on small variations.

## AES algorithm
This is a symmetric block cipher that uses a fixed block size of 128 bits and supports key sizes of 128, 192, and 256 bits. It uses a substitution-permutation network (SPN) structure that consists of 10, 12, or 14 rounds, depending on the key size. Each round consists of four operations: SubBytes, ShiftRows, MixColumns, and AddRoundKey. The S-Box is a 256-byte substitution table that is used in the SubBytes operation to perform a byte-by-byte substitution of the state. The key expansion mechanism is a process that generates a series of round keys from the main key using a recursive algorithm. The initial permutation is the first AddRoundKey operation that XORs the state with the first round key. The final permutation is the last round that omits the MixColumns operation.

## Four operations of AES
- **SubBytes**: This operation uses the S-Box to perform a non-linear substitution of each byte in the state, increasing the confusion of the cipher.
- **ShiftRows**: This operation cyclically shifts each row of the state by a certain offset, increasing the diffusion of the cipher.
- **MixColumns**: This operation performs a matrix multiplication of each column of the state with a fixed polynomial, increasing the diffusion of the cipher.
- **AddRoundKey**: This operation XORs the state with the round key, providing the only source of key mixing in the cipher.

## Differences between AES and DES
- **Key size**: AES supports larger key sizes than DES, which only has a 56-bit key. This makes AES more resistant to brute-force attacks than DES.
- **Block size**: AES has a larger block size than DES, which only has a 64-bit block. This makes AES more efficient and secure than DES, as it can process more data in less time and avoid some modes of attack that exploit small block sizes.
- **Algorithm structure**: AES uses a SPN structure, while DES uses a Feistel structure. This means that AES operates on the entire data block in every round, while DES operates on half of the data block in every round. This also means that AES does not have a decryption algorithm that is the inverse of the encryption algorithm, while DES does.
- **Number of rounds**: AES has more rounds than DES, which only has 16 rounds. This makes AES more secure than DES, as it provides more opportunities for mixing the plaintext and the key.
