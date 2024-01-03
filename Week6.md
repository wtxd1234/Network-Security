## Hash Function
- A hash function is a __mathematical function__ that __takes an arbitrary input__ (called a message) and __produces a fixed-length output__ (called a hash or a digest). A hash function has the following properties:
    - It is __easy to compute__ the hash value for any given message.
    - It is __infeasible不可能 to find a message that has a given hash value__ (preimage resistance).
    - It is __infeasible to find two different messages that have the same hash value__ (collision resistance).
    - A __small change in the message should result in a significant change in the hash value__ (avalanche effect).

- A hash function can __provide security services__ such as data integrity, message authentication, digital signatures, and pseudorandomness.

## Hash Functions Applications in Real-World 
- __Message Authentication Codes (MACs)__: A MAC is a hash value that is __computed using a secret key and appended to a message__.
  - The __receiver can verify the authenticity and integrity of the message by recomputing the MAC using the same key and comparing it with the received MAC__.
- __Digital Signatures__: A digital signature is a __hash value__ that is __encrypted using the sender's private key__ and __attached to a message__.
  - The __receiver can verify the authenticity and integrity of the message by decrypting the signature using the sender's public key__ and __comparing it with the hash value of the message__.
- __Password Storage__: A password can be __hashed and stored in a database__ instead of storing it in plaintext.
  - This way, even if the database is compromised, the attacker cannot recover the original password from the hash value.
  - To __authenticate a user__, the system can __hash the entered password and compare it with the stored hash value__.
- __Intrusion Detection and Virus Detection__: A hash value can be used to __identify a file or a program__ and __detect any unauthorized changes or modifications__.
  - For example, an antivirus software can compare the hash values of the files on a system with a database of known hash values of malicious files and alert the user if any match is found.
- Pseudorandom Function (PRF) and Pseudorandom Number Generator (PRNG): A PRF is a function that takes an input and produces an output that is indistinguishable from random.
  - A PRNG is a function that generates a sequence of numbers that are indistinguishable from random.
  - A hash function can be used to construct a PRF or a PRNG by applying it to a secret key and a counter or a seed value.

## Security Properties of Hash Function
- Preimage resistance, second preimage resistance, and collision resistance are three security properties of a hash function that measure its resistance to different types of attacks. They are defined as follows:
    - Preimage resistance: A hash function H is preimage resistant if, given a hash value h, it is infeasible to find a message M such that H(M) = h. This property prevents an attacker from finding the original message from a given hash value.
    - Second preimage resistance: A hash function H is second preimage resistant if, given a message M, it is infeasible to find another message M' such that H(M) = H(M'). This property prevents an attacker from finding a different message that has the same hash value as a given message.
    - Collision resistance: A hash function H is collision resistant if it is infeasible to find any two messages M and M' such that H(M) = H(M'). This property prevents an attacker from finding any pair of messages that have the same hash value.
