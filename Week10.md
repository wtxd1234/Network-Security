## SSL/TLS Protocols
- **SSL/TLS protocols**: They are protocols that provide security services to application layer protocols using TCP, such as HTTP, SMTP, FTP, etc¹[1]. They encrypt the data exchanged between the client and the server, authenticate the entities using certificates, and ensure the integrity of the messages using MACs.

## Firewall rules
- **Firewall rules**: They are rules that specify the action to be taken for each incoming or outgoing packet based on the source and destination IP addresses, ports, protocols, and other criteria. A firewall table is a data structure that stores the firewall rules and matches them with the packets. A possible firewall table is:

| Source IP | Destination IP | Source Port | Destination Port | Protocol | Action |
| --- | --- | --- | --- | --- | --- |
| 10.0.0.1 | Any | Any | 80 | TCP | Allow |
| 10.0.0.2 | Any | Any | 443 | TCP | Allow |
| 10.0.0.3 | Any | Any | 25 | TCP | Allow |
| Any | 10.0.0.4 | Any | 53 | UDP | Allow |
| Any | Any | Any | Any | Any | Deny |

## PGP and S/MIME
- **PGP and S/MIME**: They are standards for providing confidentiality and authentication for electronic mail systems. They use public-key cryptography and digital signatures to encrypt and sign the email messages. PGP is an open and decentralized system, while S/MIME is a centralized and standardized system. Both systems rely on certificates to verify the public keys of the entities.
