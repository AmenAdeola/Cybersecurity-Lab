# Data Leak Analysis

## Objective

Analyze a data leak incident and evaluate how the principle of least privilege could have prevented the unauthorized disclosure of confidential information.
---------

## Incident Summary

A sales manager shared access to a folder containing internal-only documents with members of the sales team.

The folder contained:
-  Product development information
-  Customer analytics
-  Marketing materials

After the meeting, access to the folder was not removed.
  

During a video call with a business partner, a member of the sales team forgot the warning from their manager. The sales representative intended to share a link to the promotional materials so that the business partner could circulate the materials to their customers. However, the sales representative accidentally shared a link to the internal folder instead. Later, the business partner posted the link on their company's social media page assuming that it was the promotional materials.

--------
## Issue
The principle of least privilege was not properly enforced. Employees retained access to internal documents after the meeting even though access was no longer required. The sales representative was able to share an entire internal folder instead of only the approved marketing materials, which contributed to the data leak.

---------

## Review
NIST SP 800-53: AC-6 focuses on the principle of least privilege , Users should only receive the minimum access required to perform their job functions. Access rights should be controlled, monitored, reviewed, regularly, and removed when no longer necessary.

--------
## Recommendations
1- Restrict access to sensitive resources based on user roles.
2- Automatically revoke temporary access after a defined period of time

--------------
## Justification
Role-based access controls would ensure that employees only have access to information necessary for their responsibilities. Automatic removal of temporary permissions would reduce the risk of unnecessary access remaining active after meetings or projects. Together, these controls would significantly reduce the likelihood of accidental data exposure.

## Key Takeaways
-  Least privilege reduces exposure to sensitive information
-  Temporary access should be revoked when no longer required
-  role-based access controls help prevent unauthorized disclosure
-  Data privacy depends on proper access management.
-  NIST SP 800-53 AC-6 provides guidance for implementing least privilege controls.

## Skills  Demonstrated
-  Access Control Analysis
-  Information Privacy
-  NIST SP 800-53 compliance
-  Data Leak Prevention
-  Risk Reduction
-  Security Governance





