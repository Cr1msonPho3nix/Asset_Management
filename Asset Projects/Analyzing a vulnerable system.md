# Scenario
You are a newly hired cybersecurity analyst for an e-commerce company. The company stores information on a remote database server, since many of the employees work remotely from locations all around the world. Employees of the company regularly query, or request, data from the server to find potential customers. The database has been open to the public since the company's launch three years ago. As a cybersecurity professional, you recognize that keeping the database server open to the public is a serious vulnerability.

You are tasked with completing a vulnerability assessment of the situation to communicate the potential risks to decision makers at the company. You must create a written report that explains how the vulnerable server is a risk to business operations and how it can be secured.

## Vulnerability Assessment Report
### System Description
The server hardware consists of a powerful CPU processor and 128GB of memory. It runs on the latest version of Linux operating system and hosts a MySQL database management system. It is configured with a stable network connection using IPv4 addresses and interacts with other servers on the network. Security measures include SSL/TLS encrypted connections.

### Scope
The scope of this vulnerability assessment relates to the current access controls of the system. The assessment will cover a period of three months, from June 2024 to August 2024. NIST SP 800-30 Rev. 1 is used to guide the risk analysis of the information system.

### Purpose
- How is the database server valuable to the business?
The database is crucial for the business, cause it stores the information and its accessed by many employees around the world.

- Why is it important for the business to secure the data on the server?
To prevent threat actors to access the information withing the server.

- How might the server impact the business if it were disabled?
The data could be compromised and the employees couldn't connect to it to work, which means a stop in the workflow of the business.

### Risk Assessment

| Threat Source | Threat Event | Likelihood | Severity | Risk |
|--             |--            |--          |--        |--    |
| Cybercriminal | Obtanining crucial information from the business and leaking or selling it | 3 | 3 | 9 |
| Cybercriminal | Encryption of the database with a ramsonware to ask the business for money | 3 | 3 | 9 |
| Cybercriminal | Manipulating information within the database to further expand control over internal network | 3 | 3 | 9 |
| Insider       | Obtanining crucial information from the business and leaking or selling it | 2 | 3 | 6 |
| Costumer      | Manipulating information for benefits                                      | 1 | 2 | 2 |

### Remediation Strategy
An implementation of various methods are in order:
- First and most important, change the privacity of the database so only the members of specific groups can access it.
- Create those groups, giving them the proper privileges.
- MFA authentication must be implemented to ensure the authenticity of the person.
- Data Encryption should be implemented if the data of the server is plain-text, as another layer of protection against cybercriminals.