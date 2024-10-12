# Scenario

You work for an educational technology company that developed an application to help teachers automatically grade assignments. The application handles a wide range of data that it collects from academic institutions, instructors, parents, and students.

Your team was alerted to a data leak of internal business plans on social media. An investigation by the team discovered that an employee accidentally shared those confidential documents with an external business partner. An audit into the leak is underway to determine how similar incidents can be avoided.

A supervisor provided you with information regarding the leak. It appears that the principle of least privilege was not observed by employees at the company during a sales meeting. You have been asked to analyze the situation and find ways to prevent it from happening again.

## Incident Summary
A sales manager shared access to a folder of internal-only documents with their team during a meeting. The folder contained files associated with a new product that has not been publicly announced. It also included customer analytics and promotional materials. After the meeting, the manager did not revoke access to the internal folder, but warned the team to wait for approval before sharing the promotional materials with others.

During a video call with a business partner, a member of the sales team forgot the warning from their manager. The sales representative intended to share a link to the promotional materials so that the business partner could circulate the materials to their customers. However, the sales representative
accidentally shared a link to the internal folder instead. Later, the business partner posted the link on their company's social media page assuming that it was the promotional materials.<br>

| Control | Least Privilege |
|--       |--               |
| Issues | What factors contributed to the information leak?<br>1. Not revoking access to the shared folder by sales manager.<br>2. The sales representative sharing the wrong link before checking if it was the correct one. |
| Review | What does NIST SP 800-53: AC-6 address?<br>- It addresses how organizations can use the "Least Privilege" to prevent access to users without authorization. The intention is to prevent a user from operating at privilege levels higher than what is necessary to accomplish business objectives.  |
| Recommendations | How might the principle of least privilege be improved at the company?<br>By:<br>- Restricting access to sensitive resources based on user role.<br>- Automatically revoke access to information after a period of time.<br>- Regularly audit user privileges.  |
| Justification | How might these improvements address the issues?<br>By giving strict access to a set users can prevent data leak, as the permission needed to see the data with the shared link. Also, security teams should check if those permissions are checked on a basis to prevent privilege creep on users. |