# Organ-Transplantation-Network
This is my DBMS course project.
Project work carried out on flask and mysql(Database management system  Project).Develop an online portal using flask and html:-

=> To keep a track of each organ donated by donor and the organ transplanted into the patient. Thus, creating a transparent and user friendly website for Organ transplantation Management system.

=> To reduce the prevailing malpractices.

=>To reduce the wastage of organs due to lack of proper database management system.

=> To create live statistics of donors (graph between successful and failed transplantation) .

MYSQL CONNECTION:-
1-run all the queries given in create_tables.sql file in your mysql database.By creating the database name "DBMS_PROJECT".
2-after that run all queries of insertions present in inserting_data folder run quries present in all sql file in that folder.
3-change some configuration in app.py file to connect mysql database with your project :-(from line-7 to line-12)
mydb = mysql.connector.connect(
  host='localhost',
  user='root',
  password='<password of your own mysql server>',
  database = 'DBMS_PROJECT'
) 

Python Settings:-
1-Install Python -version 3.8.0 with add to path.
2-Install required libraries given in requirements.txt file.
3-For installing libraries individually type command line "pip install <package name>".(flask,mysql.connector,matplotlib,hashlib,numpy,pyrebase4) this are main packages pip install this all packages and some dependency packages also.
4-To install all libraries together type command line "pip install -r requiremnts.txt" by changing directory to the folder where you have save requirements.txt(This file itself present in the unziped folder) file.(if suppose some error occured install packages manually by following third step)
5-change the directory to the Unziped folder and type  command line "python app.py" in command prompt to run project(to run app.py file).
7-The project will run on your localhost-5000 server.
8-For admin portal -- username is "admin" password is "admin".
9-For public portal normal sign-in and sign-up system.(for public portal the google firebase id used which will get expired in 30 days ,to change it with new configuration add your own api keys and other firebase configuration and allow your firebase project for authentication)
  
***If you are using pycharm just install required packages in your python interpreter or in virtual environment(if you have created any) and just run app.py file*** 


Firebase settings(if sign-up and sign-in for public portal is not working then change firebase configuration:-
Practice this step only if public portal is not working.
1-create account on google firebase
2-create new project enable authentication syatem in authentication->email/password section
3-In project overview section create a new app and just replace all the configuration with new ones. 
change this lines in app.py according to your configuration:
config = {
    "apiKey": "AIzaSyD06kI5ACT1GDMrIs6N035mu8bAIEF-rDA",
    "authDomain": "dbms-project-9fab5.firebaseapp.com",
    "databaseURL": "https://dbms-project-9fab5.firebaseio.com",
    "projectId": "dbms-project-9fab5",
    "storageBucket": "dbms-project-9fab5.appspot.com",
    "messagingSenderId": "191339204412",
    "appId": "1:191339204412:web:44758ee2be680db12e9839"
}
