About:
======

The TIMELINE FOLLOWBACK (TLFB) is an interview-based assessment that was developed and copyrighted by Sobell & Sobell (2000). The TLFB derives subjects' retrospective daily estimates of alcohol consumption patterns. Using a calendar as a visual aid, special events, and other memory cues, subjects are guided through the process of recalling and reporting daily drinking estimates.


Installation:
============

1. Download the zip file above and unzip it or you can down the two files (a)calendarSurveyScript (b)calendarSurveySouceCode to your web server.
2. Open MS SQL Server.
3. Create a new database "calendarSurvey".  
4. Open Notepad, copy, paste and run the CalendarSurveyScript.sql on the new "calendarSurvey" database created above.
5. In MSSQL, create a new account with a role as database owner for the new database "CalendarSurvey".
6. In MSSQL, use the "CalendarSurvey" database, open table "investigators". This is the table where you use to enter new login ID and password for new participant ID.
7. In table "investigators" add a new row with the following data: user name "admin" to column "username" and password "password" to column "password", a start date e.g. "10/20/2013" to column "startDate", an end date e.g. "12/12/2013" and "21" to column "role".
8. Unzip the "CalendarSurveySourceCode" to your web server root directory. Copy this folder "carl" to your web root directory . Normally the web root directory is located in c:/inetpub/www/
9. Modify the "web.config" file which is located in the root directory of the unzip "calendarSurveySourceCode" and look for the following line and change the properties for the databsse connection string.

         <add key="ConnectionString" value="server=yourDatabaseServerIPAddress;uid='LoginIDForTheCalendarSurvey';password='PasswordForTheCalendarSurvey';initial catalog='NameOfCalendarSurveyDatabase' "/>

In the above connection string replace 
1. "yourDatabaseServerIPAddress" with your database server IP address,
2. "uid" with the login ID you created in step 4 above
3. "PasswordForTheCalendarSurvey" with the password for the account you created in step 4 above
4. "NameOfCalendarSurveyDatabase" with the name of the databbase you created in step 3 above.


Author:
======

Kevin Le, MS, Center for Research Informatics, University of Chicago

If you have any questions about the coding or installation, please contact

Kevin Le, MS, University of Chicago
5751 S. Woodlawn Dr. Suite 404
Chicago, IL. 60637
Email: kle@bsd.uchicago.edu
Phone: 773 484 8841


Copyright and License information:
=================================

The code for the Online TLFB (O-TLFB) is copyright pending by Kevin Le, MS, Center for Research Informatics, University of Chicago

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, and/or modify copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright pending notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


Acknowledgements:
================

Appreciation is extended to Patrick McNamara and Andrea King, Department of Psychiatry and Behavioral Neuroscience, The University of Chicago, Chicago, Illinois, and Sandra Yu Rueger, Department of Psychology, Wheaton College, Wheaton, Illinois for their guidance with study design and implementation of the self-administered web-based O-TLFB


The Center for Research Informatics is funded by the Biological Sciences Division at the University of Chicago with additional funding provided by the Institute for Translational Medicine, CTSA grant number UL1 RR024999 from the National Institutes of Health.

Commit summary: Extended description: (optional)
kle1999 minhkevin@gmail.com
