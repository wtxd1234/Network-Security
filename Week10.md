## SSL/TLS Protocols
- **SSL/TLS protocols**: They are protocols that __provide security services to application layer protocols using TCP__, such as HTTP, SMTP, FTP, etc. They __encrypt the data exchanged__ between the client and the server, __authenticate the entities using certificates__, and __ensure the integrity of the messages using MACs__.

## Firewall rules
- **Firewall rules**: They are __rules that specify the action to be taken for each incoming or outgoing packet__ based on the source and destination IP addresses, ports, protocols, and other criteria.
- **Firewall table**: It is a __data structure that stores the firewall rules and matches them with the packets__. A possible firewall table is:

| Source IP | Destination IP | Source Port | Destination Port | Protocol | Action |
| --- | --- | --- | --- | --- | --- |
| 10.0.0.1 | Any | Any | 80 | TCP | Allow |
| 10.0.0.2 | Any | Any | 443 | TCP | Allow |
| 10.0.0.3 | Any | Any | 25 | TCP | Allow |
| Any | 10.0.0.4 | Any | 53 | UDP | Allow |
| Any | Any | Any | Any | Any | Deny |

## PGP and S/MIME
- **PGP and S/MIME**: They are __standards for providing confidentiality and authentication for electronic mail systems__.
- They use __public-key cryptography and digital signatures to encrypt__ and __sign the email messages__.
- __PGP__ is an __open and decentralized system__, while __S/MIME__ is a __centralized and standardized system__.
- Both systems __rely on certificates to verify the public keys of the entities__.
