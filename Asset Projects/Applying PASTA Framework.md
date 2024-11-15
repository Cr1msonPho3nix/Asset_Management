# Scenario
You’re part of the growing security team at a company for sneaker enthusiasts and collectors. The business is preparing to launch a mobile app that makes it easy for their customers to buy and sell shoes.

You are performing a threat model of the application using the PASTA framework. You will go through each of the seven stages of the framework to identify security requirements for the new sneaker company app.

## App information
- Our application should seamlessly connect sellers and shoppers. It should be easy for users to sign-up, log in, and manage their accounts. Data privacy is a big concern for us. We want users to feel confident that we’re being responsible with their information.<br><br>
- Buyers should be able to directly message sellers with questions. They should also have the ability to rate sellers to encourage good service. Sales should be clear and quick to process. Users should have several payment options for a smooth checkout process. Proper payment handling is really important because we want to avoid legal issues.<br><br>
- The app will be exchanging and storing a lot of user data. These are some of the technologies that it uses:
  - Application programming interface (API): An API is a set of rules that define how software components interact with each other. In application development, third-party APIs are commonly used to add functionality without having to program it from scratch.
  - Public key infrastructure (PKI): PKI is an encryption framework that secures the exchange of online information. The mobile app uses a combination of symmetric and asymmetric encryption algorithms: AES and RSA. AES encryption is used to encrypt sensitive data, such as credit card information. RSA encryption is used to exchange keys between the app and a user's device.
  - SHA-256: SHA-256 is a commonly used hash function that takes an input of any length and produces a digest of 256 bits. The sneaker app will use SHA-256 to protect sensitive user data, like passwords and credit card numbers.
  - Structured query language (SQL): SQL is a programming language used to create, interact with, and request information from a database. For example, the mobile app uses SQL to store information about the sneakers that are for sale, as well as the sellers who are selling them. It also  uses SQL to access that data during a purchase.<br>

## PASTA Worksheet
| Stages | Sneaker Company |
|--      |--               |
| 1. Define business and security objectives | - The app was created as an easily way to connect sellers and shoppers.<br>- Shoppers rating sellers easily to encourage a better service.<br>- Several payment options and proper payment handling is crucial to avoid legal issues. |
| 2. Define the technical scope | - API is used to set the rules to communicate.<br>- PKI is implemented for encryption purposes.<br>- SHA-256 is a hash function that will be used to protect PII.<br>- SQL is used to access all the data about the sneakers sold and bought. |
| 3. Decompose application | ![PASTA_diagram](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/PASTA%20Framework/1.1.PASTA_dataflow_diagram.PNG) |
| 4. Threat analysis | - Stealed Credentials from Shoppers or Admins.<br>- DoS by interrupting the flow to the Database.<br>- Prone to SQL injection if no protection method is included. |
| 5. Vulnerability analysis | - No MFA or low security credential policy.<br>- Server being overwhelmed by traffic from one or more machines.<br>- SQL injection caused of no implementation of prepared statements, input sanitization or input validation.  |
| 6. Attack modeling | ![PASTA_attack_tree](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/PASTA%20Framework/2.1.PASTA_attack_tree.PNG) |
| 7. Risk analysis and impact | - Password policies and MFA implemented.<br>- Secured development of the APP, including previously SQL methods discussed.<br>- Hashing and encrypting the information, in case of a successful attack.<br>- Preventing a DoS attack by diverting the extra traffic. <br>- Creation of a playbook in case of an event happening. |