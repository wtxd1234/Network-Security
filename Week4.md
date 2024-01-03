## Avalanche effect
- This is the property that a __small change in the plaintext or the key__ result in a __significant change in the ciphertext__.
- It contributes to __enhance security__ by making it harder for attackers to use __cryptanalysis methods to uncover the original plaintext or key__, as they __cannot predict how the ciphertext will change based on small variations__.

## AES algorithm
- This is a __symmetric block cipher__ that uses a __fixed block size of 128 bits__ and __supports key sizes of 128, 192, and 256 bits__.
- It uses a __substitution-permutation network (SPN) structure__ that consists of __10, 12, or 14 rounds__, depending on the __key size__.
- Each round consists of __four__ operations: __SubBytes, ShiftRows, MixColumns__, and __AddRoundKey__.
- The __S-Box__ is a __256-byte substitution table__ that is used in the __SubBytes__ operation to __perform a byte-by-byte substitution__ of the state.
- The __key expansion mechanism__ is a process that __generates a series of round keys from the main key__ using a __recursive algorithm__.
- The __initial permutation__ is the __first AddRoundKey operation__ that __XORs__ the state with the __first round key__.
- The __final permutation__ is the __last round__ that omits the __MixColumns operation__.

## Four operations of AES
- **SubBytes**: This operation uses the __S-Box__ to perform a __non-linear substitution of each byte__ in the state, increasing the __confusion__ of the cipher.
- **ShiftRows**: This operation __cyclically shifts each row of the state by a certain offset__, increasing the __diffusion__ of the cipher.
- **MixColumns**: This operation performs a __matrix multiplication of each column of the state with a fixed polynomial__, increasing the __diffusion__ of the cipher.
- **AddRoundKey**: This operation __XORs__ the state with the round key, providing the __only source of key mixing in the cipher__.

## Differences between AES and DES
- **Key size**: AES supports __larger key sizes than DES__, which only has a 56-bit key. This makes AES __more resistant to brute-force attacks than DES__.
- **Block size**: AES has a __larger block size than DES__, which only has a 64-bit block. This makes AES __more efficient and secure than DES__, as it can process more data in less time and avoid some modes of attack that exploit small block sizes.
- **Algorithm structure**: AES uses a __SPN structure__, while DES uses a __Feistel structure__. This means that AES operates on the __entire data block in every round__, while DES operates on __half of the data block in every round__. This also means that __AES does not have a decryption algorithm__ that is the inverse of the encryption algorithm, while DES does.
- **Number of rounds**: AES has __more rounds than DES__, which only has 16 rounds. This makes AES __more secure than DES__, as it provides __more opportunities for mixing the plaintext and the key__.
