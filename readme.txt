This work is provided for free distribution by Kevin Le, Patrick McNamara,
Sandra Yu Rueger, PHD, Constantine J.Trela, B.A, Michael Palmeri, B.S, and Andrea C. King Ph.D

Center for Research Informatics, The University of Chicago, Chicago, Illinois
Department of Psychiatry and Behavioral Neuroscience, Pritzker School of Medicine, 
The University of Chicago, Chicago, Illinois; 
Department of Psychology, Wheaton College, Wheaton, Illinois

Please see Copyright and License below for more details

About:
======

The TIMELINE FOLLOWBACK (TLFB) is an interview-based assessment that was developed by Sobell et al. (1986) to 
derive subjects' retrospective daily estimates of alcohol consumption patterns. Using a calendar as a visual aid,
special events, and other memory cues, subjects are guided through the process of recalling and reporting daily 
drinking estimates.



Installation:
============

1. Download the follwow two files (a)calendarSurveyScript (b)calendarSurveySouceCode
2. Open MS SQL Server.
3. Open Notepad, Copy and paste the CalendarSurvey script to the SQL server to create a new "CalendarSurvey" database.
4. Grant proper user name and password to the new database.
5. Unzip the "CalendarSurveySourceCode" to your web server root directory. Rename this directory as your choice.
 Normally the web root directory is located in c:/inetpub/www/
6. Modify the "web.config" file which is located in the root directory of the unzip "calendarSurveySourceCode" and look for the following line and change the property for the databse connection.

         <add key="ConnectionString" value="server=yourDatabaseServerIPAddress;uid='LoginIDForTheCalendarSurvey';password='PasswordForTheCalendarSurvey';initial catalog='NameOfCalendarSurveyDatabase' "/>


Author:
=======

Kevin Le, MS, University of Chicago

If you have any question, please contact Kevin Le via email at

Email: kle@bsd.uchicago.edu or minhkevin@gmail.com

Phone: 773 484 8841 or 773 279 1816


Copyright and License
=====================

Copyright (c) 2013 Kevin Le

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
