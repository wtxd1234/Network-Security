## Define hash function and its roles in providing security services.
- A hash function is a mathematical function that takes an arbitrary input (called a message) and produces a fixed-length output (called a hash or a digest). A hash function has the following properties:
    - It is easy to compute the hash value for any given message.
    - It is infeasible to find a message that has a given hash value (preimage resistance).
    - It is infeasible to find two different messages that have the same hash value (collision resistance).
    - A small change in the message should result in a significant change in the hash value (avalanche effect).

- A hash function can provide security services such as data integrity, message authentication, digital signatures, and pseudorandomness.

## Name hash functions applications in real-world. 
- Some real-world applications of hash functions are:
    - Message Authentication Codes (MACs): A MAC is a hash value that is computed using a secret key and appended to a message. The receiver can verify the authenticity and integrity of the message by recomputing the MAC using the same key and comparing it with the received MAC.
    - Digital Signatures: A digital signature is a hash value that is encrypted using the sender's private key and attached to a message. The receiver can verify the authenticity and integrity of the message by decrypting the signature using the sender's public key and comparing it with the hash value of the message.
    - Password Storage: A password can be hashed and stored in a database instead of storing it in plaintext. This way, even if the database is compromised, the attacker cannot recover the original password from the hash value. To authenticate a user, the system can hash the entered password and compare it with the stored hash value.
    - Intrusion Detection and Virus Detection: A hash value can be used to identify a file or a program and detect any unauthorized changes or modifications. For example, an antivirus software can compare the hash values of the files on a system with a database of known hash values of malicious files and alert the user if any match is found.
    - Pseudorandom Function (PRF) and Pseudorandom Number Generator (PRNG): A PRF is a function that takes an input and produces an output that is indistinguishable from random. A PRNG is a function that generates a sequence of numbers that are indistinguishable from random. A hash function can be used to construct a PRF or a PRNG by applying it to a secret key and a counter or a seed value.

## Define preimage resistance, second preimage resistance, and collision resistance.
- Preimage resistance, second preimage resistance, and collision resistance are three security properties of a hash function that measure its resistance to different types of attacks. They are defined as follows:
    - Preimage resistance: A hash function H is preimage resistant if, given a hash value h, it is infeasible to find a message M such that H(M) = h. This property prevents an attacker from finding the original message from a given hash value.
    - Second preimage resistance: A hash function H is second preimage resistant if, given a message M, it is infeasible to find another message M' such that H(M) = H(M'). This property prevents an attacker from finding a different message that has the same hash value as a given message.
    - Collision resistance: A hash function H is collision resistant if it is infeasible to find any two messages M and M' such that H(M) = H(M'). This property prevents an attacker from finding any pair of messages that have the same hash value.
