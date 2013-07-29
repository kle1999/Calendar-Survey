This work is provided for free distribution by Kevin Le,MS. University of Chicago. You may download and use the code as your own risk.



Calendar Survey installation:

1. Download the follwow two files (a)calendarSurveyScript (b)calendarSurveySouceCode
2. Open MS SQL Server.
3. Open Notepad, Copy and paste the CalendarSurvey script to the SQL server to create a new "CalendarSurvey" database.
4. Grant proper user name and password to the new database.
5. Unzip the "CalendarSurveySourceCode" to your web server root directory. Rename this directory as your choice.
 Normally the web root directory is located in c:/inetpub/www/
6. Modify the "web.config" file which is located in the root directory of the unzip "calendarSurveySourceCode" and look for the following line and change the property for the databse connection.

         <add key="ConnectionString" value="server=yourDatabaseServerIPAddress;uid='LoginIDForTheCalendarSurvey';password='PasswordForTheCalendarSurvey';initial catalog='NameOfCalendarSurveyDatabase' "/>

If you have any question, please contact Kevin Le via email at


Email: kle@bsd.uchicago.edu or minhkevin@gmail.com

Phone: 773 484 8841 or 773 279 1816
