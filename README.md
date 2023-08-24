# IzZyCRM
 
#### Python based open source CRM developed using Flask framework

##### This is a fork of EeazyCRM, see the link below to see the original code
https://github.com/jagjot2008/EeazyCRM

##### It's still WORK IN PROGRESS


Features List
============

IzZy contains the following modules (along with the 
completion progress report):

   1. Leads (99% complete)
   2. Accounts (90% complete)
   3. Contacts (99% complete)
   4. Deals (with Pipeline view) (90% complete)
   5. Activities (still building) (Not started as yet)
   6. Reports (with charts and graph) - (60% complete)
   7. Settings (50% complete)
       1. Roles Management (100% complete)
       2. User Management (100% complete)
       3. Profile Management (100% complete)
       4. Company Management (Not started)
       5. Configuration Management (Not started)
            1. Deal Stage
            2. Lead Stage
            3. Lead Source
            4. Activity Types
            5. Email Templates
       6. Application Settings (100% complete)
   8. Invoice (Not started)
   9. Dashboard (10% complete)
   
   
Installation Requirements
============

1. Python3 (3.9+ or greater)
2. Postgresql (ver 11+ or greater)
2. pip3
3. virtualenv

Make sure that the postgresql instance is up and running.

Open the command prompt or terminal and 
create a new database with the following commands.
    
    
        psql
        create database eeazy_crm

Installation Steps
============

1. Create a virtual environment using the following commands
    
        virtualenv -p python3 eeazycrm
        source eeazycrm/bin/activate
        
2. Add github repository using the following command
    
        cd eeazycrm
        git remote add origin https://github.com/jagjot2008/EeazyCRM
        git pull origin master
        
3. Now create the configuration file using the command
    
        cp config_vars.example config_vars.py
        
    Open the config_vars.py file and add the database connection 
    parameters in the PRODUCTION DATABASE SETTINGS (Default).
    
    You can also setup the development and testing settings if you wish to.
        
3. Install the dependencies

       pip3 install -r requirements.txt

4. Create the following environment variables
   
       EMAIL_USER = <your username>
       EMAIL_PASS = <your password>
       
   If you want to run flask in development or testing mode set
   the following environment variable in addition to the above.
   
       FLASK_ENV = development, or
       FLASK_ENV = testing
   
5. Run the command
   
       python3 run.py
       
   This will run the installation wizard. Follow the instructions
   in the wizard and after finishing installation, stop the 
   application and start again by running the command in step #6.
   
That's it folks. Your CRM is running.

Report a Bug or Request a New Feature
================================

For reporting bugs in the system, you can raise a github issue or even request
a new feature.

Updates
================================
2023-08-23 Update all librarys to newest, adjust some bugs.


To-Dos
================================
1. Adjust Docker and docker-compose