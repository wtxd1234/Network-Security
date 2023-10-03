# Introduction
## Cybersecurity

- Cybersecurity is the practice of protecting critical systems and sensitive information from digital attacks.
- Cybersecurity measures are designed to combat threats against networked systems and applications.

## Cybersecurity Subsets

- ___Information security___:
  - refers to the preservation of confidentiality, integrity, and availability of __information__.
  - Additionally, authenticity, accountability, nonrepudiation, and reliability can also be involved.

- ___Network security___ :
  - Protecting the __networks and their services__ from unwanted users, attacks, and intrusions.
 
## Security Key Principle/Objectives:

![image](https://github.com/wtxd1234/Network-Security/assets/41671135/d00bf32c-4883-4c32-a0ee-12f632271e81)

## Security Principle: CIA Triad

- __Confidentiality__: Preserving __unauthorized access__ to the data.
  - Data Confidentiality
  - Privacy

- __Integrity__: Assures that data are __changed__ only in a specified and authorized manner.
  - Data Integrity
  - System Integrity
 
- __Availability__: Authorized users should be __able to access data all the time__. The systems and services are not denied to authorized users.

## Additional Security Principle

- __Authenticity真实性__: Being __genuine真实__ and being able to be verified and trusted.

- __Accountability可追踪性__: __Tracing__ the entity (have particular responsibilities).

## Essential Objectives of Information and Network Security

![image](https://github.com/wtxd1234/Network-Security/assets/41671135/2ff16f01-35bf-49e4-8580-5f3dd9bcd0a5)

## CIA Triad ATM Example

- It provides __confidentiality__ by requiring two-factor __authentication__
(both a physical card and a PIN code) before allowing access to
data.
- The ATM and bank software enforces data __integrity__ by ensuring
that any transfers or withdrawals made via the machine are
reflected in the accounting for the user's bank account.
- The machine provides __availability__ because it's in a public place
and is accessible even when the bank branch is closed.

## Other Security Terms

- ___Threats___: A __potential潜在__ for violation of security.
- ___Attack___: An __assault突击__ on system security that derives from an
intelligent threat.
- ___Vulnerability___: __Weakness__ in the security system that might be
exploited.
- ___Control___: An action, device, procedure, or technique that
__removes or reduces a vulnerability__.

___So, threats are blocked by controlling the vulnerabilities.___

## OSI Security Architecture

- ___ITU-T X.800___ is a standard to satisfy organization managers in
term of computer and security on their requirements.

- Vendors have developed their security features on products
and services based on this standard/framework.

3 aspects of security in ITU-T X.800 
  - ___Security attack___: Any action that __compromises the security__ of
information owned by an organization.
  - ___Security mechanism___: A process (or a device incorporating
such a process) that is designed to __detect, prevent, or recover__
from a security attack.
  - ___Security service___: A processing or communication service that
__enhances the security__ of the data processing systems and the
information transfers of an organization.

![image](https://github.com/wtxd1234/Network-Security/assets/41671135/e4f6b924-847e-4ca2-979f-2cdbb1e11cc8)

## Security Attacks
- The attacks are classified into __2 classes__:
  - ___Passive attack___: Attempts to learn or make use of information from the system but __does not affect__ system resources
    - 2 types:
      - __Release of message contents__: __monitoring__ the content to find __sensitive information__.
      - __Traffic analysis__: __monitor traffic__ (looking for __special patterns__ such as pattern of messages, password length, location and identity of communicating hosts, …)
    - __Difficult to detect cause no alteration of data__
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/18e70de1-7bad-43b9-b239-9a74cd80e37d)
  - ___Active attack___: __Altering__ the system resources and/or __affects__ on the system as well
    - Alter resources or operations
    - It involves some modification of the data stream or false statements
    - 4 types:
      1. ___Masquerade___: One entity __pretends__ to be another entity (MITM)
      2. ___Replay___: __Capture__ message and __reply__ to get authorized access
      3. ___Modification___: __Alter, reorder, and delay__ to an authorized access
      4. ___Denial of service___: __Prevents or inhibits__ the normal use or management of __communications facilities__
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/378f2f65-cd76-42e3-892f-6f6dda853d3d)
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/7006c5bf-96ad-4d7a-a07c-332574fc5d78)

## Active vs Passive Attacks
| | Active Attacks | Passive Attacks |
| :--- | :--- | :--- |
| Modification of information | ✅ | ❌ |
| Harm to the system | ✅ | ❌ |
| Victims informed by system | ✅ | ❌ |
| Counter and prevent | Difficult | Easy |

## Security Services
- ITU-T X.800 standards divide security services into __6 categories__:
  1. ___Authentication___: Assurance that the communicating entity is the one claimed
  2. ___Access control___: Prevention of the unauthorized use of a resource
  3. ___Data confidentiality___: Protection of data from unauthorized disclosure
  4. ___Data integrity___: Assurance that data received is as sent by an authorized entity
  5. ___Nonrepudiation不可否认性___: Protection against denial by one of the parties in a communication
  6. ___Availability___: Resource accessible/usable

## Security Mechanism
- ___Cryptographic algorithms___ (encipherment): The use of __mathematical algorithms__ to transform data into a form that is not __readily intelligible__
- ___Data integrity___: It covers a variety of mechanisms used to __ensure the integrity__ of a data unit or stream of data units
- ___Digital signature___: Data appended to, or a cryptographic transformation of, a data unit that allows a recipient of the data unit to __prove the source and integrity__ of the data unit and protect against __forgery伪造__
- ___Authentication exchange___: A mechanism intended to __ensure the identity__ of an entity by means of information exchange
- ___Traffic padding___: The insertion of bits into gaps in a data stream to __frustrate阻扰 traffic analysis__ attempts
- ___Routing control___: Enables selection of particular physically or logically __secure routes__ for certain data and allows routing changes, especially when a breach of security is suspected
- ___Notarization公证___: The use of a __Trusted Third Party (TTP)__ to ensure certain properties of a data exchange
- ___Access control___: A variety of mechanisms that enforce __access rights__ to resources

## Relationship Between Security Services and Mechanisms
![image](https://github.com/wtxd1234/Network-Security/assets/41671135/b5d9e1d0-978f-4b50-97fa-8254069020fc)
