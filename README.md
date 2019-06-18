# ShadowIT-Report
Scheduled SaaS Application Usage Report
The purpose of this Skillet is to automate the creation of a scheduled SaaS Application Usage Report on either the NGFW (PANOS) or on Panorama.

In order to get the most from this skillet and the report it creates, it is highly recommended that SSL Decryption be used, and all or as many security rules as possible have profiles attached configured to log as verbosely as possibly (preferably logging all). 

The skillet will perform the following tasks:
1. Create 3 detailed SaaS Application Usage Reports under the Monitor tab - SaaS Application Usage Report for trailing 7, 30, and 90 days.
2. Create an Email Server Profile under the Settings - Email Server page.  This will require a mail server which is configured to allow the NGFW or Panorama to relay mail, please see the PAN-OS Admin Guide for additional details on mail server setup requirements.
3. Create an automated scheduler which will email the selected report on a weekly schedule on Sunday so that administrators can review when arriving at work on Monday morning.

