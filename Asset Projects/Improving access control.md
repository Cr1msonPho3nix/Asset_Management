# Scenario
You’re the first cybersecurity professional hired by a growing business.

Recently, a deposit was made from the business to an unknown bank account. The finance manager says they didn’t make a mistake. Fortunately, they were able to stop the payment. The owner has asked you to investigate what happened to prevent any future incidents.

To do this, you’ll need to do some accounting on the incident to better understand what happened. First, you will review the access log of the incident. Next, you will take notes that can help you identify a possible threat actor. Then, you will spot issues with the access controls that were exploited by the user. Finally, you will recommend mitigations that can improve the business' access controls and reduce the likelihood that this incident reoccurs.

## Access Log
- Event Type: Information
- Event Source: AdsmEmployeeService
- Event Category: None
- Event ID: 1227
- Date: 10/03/2023
- Time: 8:29:57 AM
- User: Legal\Administrator
- Computer: Up2-NoGud
- IP: 152.207.255.255
- Description:
- Payroll event added. FAUX_BANK

## Employee Directory<br>
![Employee-directory](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/Improving%Access%Controls/1.1-Employee-directory.PNG)<br>

## Access Control Worksheet
### List 1-2 pieces of information that can help identify the threat:
- <b>Who caused this incident?</b>
Was caused by an Administrator user, Robert Taylor Jr., due to the "Legal" role and the IP connection.
- <b>When did it occur?</b>
10/03/2023 - At 8:29:57
- <b>What device was used?</b>
A compute with the ID "Up2-NoGud", connected with the IP "152.207.255.255"

### Based on your notes, list 1-2 authorization issues:
- <b>What level of access did the user have?</b>
High level, as Administrator.
- <b>Should their account be active?</b>
No, cause the end date of his contract figures as 12/27/2019, which is more than 3 years ago.
### Make at least 1 recommendation that could prevent this kind of incident:
- <b>Which technical, operational, or managerial controls could help?</b>
  - MFA should be implemented in case an account access was stolen.
  - Deleting (or revoking access) the accounts from users that are not actually operational in the business.
  - Using the "principle of least privilege" to grant the minimum level of permission, cause not everyone needs to be "administrator".