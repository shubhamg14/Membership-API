# Membership-API
Authentication REST API which can be used to add, update, delete member details built using Flask(jsonify), sqlite3 and deployed on Pythonanywhere.com 

## Features

1. GET "/member" - Returns all members
2. GET "/member/<int:member_id>" -  Returns that id's information
3. POST "/member" - Insert members information into database and returns what has been inserted
4. PUT/PATCH "/member/<int:member_id>" - Updates member information
5. DELETE "/member/<int:member_id>" - Delete member information of the id which has been deleted

Authentication using decorators in python via Username and Password has also been setup - Username ("admin") Password ("password")

## Deploying API on Pythonanywhere

1. Create a free begineers account(Free) on pythonanywhere.com
2. Go to Bash
3. Create virtual environment ("mkvirtualenv --python=/usr/bin/python3.4 env")
4. Install Flask("pip install flask")
5. Clone github repository ("git clone <repository-name>")
6. Go to console and kill bash session
7. Go to Web tab and click "Add a new web page"
8. Click next when web address displays and then Select Manual configurationand select preferred python version.
9. When the setup is complete, go to Virtual Environment tab and enter env and it will automatically fill the virtual environmebt we created
10. Go to WSGI configuration file and make following changes
    ![alt text](https://github.com/shubhamg14/Membership-API/blob/master/images/Wsgi-Membership-Api.PNG)
11. Change the path of members.db file in database file to point to correct path on pythonanywhere.com  
12. Go back to dashboard and reload your webpage. 

## Validating API

Go to the link of pythonanywhere website and using POSTMAN send data over the endpoints and validate
