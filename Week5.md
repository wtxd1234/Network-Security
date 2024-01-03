## Block Ciphers vs Stream Ciphers 
- Block ciphers operate on __fixed-length blocks of plaintext__, while stream ciphers operate on __individual bits or bytes of plaintext__.
- __Block ciphers__ are more suitable for applications that __require random access__, such as __disk encryption__ or __file encryption__.
- __Stream ciphers__ are more suitable for applications that __require sequential processing__, such as __communication channels__ or __streaming media__.

## Two Operators in RC4 
- __XOR__ is used to __combine the keystream with the plaintext__ to __produce the ciphertext__, and vice versa.
- __Swap__ is used to __permute the state vector S__, which is used to __generate the keystream__.

## Practical Scenarios for Block Ciphers and Stream Ciphers
- __Block ciphers__ are commonly used in __symmetric encryption algorithms__, such as __AES, DES,__ and __3DES__. They are also used in __modes of operation__, such as __CBC, CTR,__ and __GCM__, to __provide various security properties__, such as __confidentiality, integrity,__ and __authentication__.
- __Stream ciphers__ are commonly used in __wireless security protocols__, such as __WEP, WPA,__ and __Bluetooth__. They are also used in __SSL and TLS protocols__ to __provide secure communication__ between web browsers and servers.

## Constraints for True Random Number Generator 
- A __true random number generator (TRNG)__ must __produce output that is unpredictable, unbiased, and independent__. This means that the __output cannot be determined by any previous or future values__, that the output has a __uniform distribution__, and that the output is __not correlated with any other variables__.
- However, achieving these properties is challenging, as most __physical sources of randomness__ are subject to __noise, interference, and degradation__. Therefore, TRNGs often __require complex hardware design, calibration, and testing__ to ensure their __quality and reliability__.

## Advantages and Disadvantages of RC4 
- __Advantage__: __speed, simplicity,__ and __low memory requirement__.
  - It is easy to implement and can run efficiently on various platforms.
- __Disadvantages__: __vulnerabilities, security weaknesses,__ and __lack of standardization__.
  - RC4 has several known attacks that can exploit its flaws in the keystream generation, the state initialization, and the key scheduling.
  - RC4 also has some inherent weaknesses in its design, such as biases, correlations, and repetitions in the keystream.
  - RC4 is not a standardized algorithm, and different implementations may have different specifications and parameters.
