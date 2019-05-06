# Personalized-Meal-Plan-Subscription

Ensure the following packages are installed in the execution environment:

1.	MySQL server
Install community Server
Install Workbench

2.	Mongo DB: should be installed without setting password option
Install Mongodb

3.	Node.js and NPM 
Install node and npm

4.	IDE (any compatible IDE)
Install visual studio code

 ****************************** Folder Structure  ******************************

      1. DB Application Directory: This directory contains the following folders:
      ●	app_server : contains server page, router page and all the application pages
      ●	log : log file will be generated into this folder
      ●	public : contains the home page of the application
      ●	app.js 
      ●	package.json : dependencies 

      2. SQL Directory:
      ●	Insert_Statements.sql
      ●	Stored_procedures_admin.sql
      ●	Stored_procedures_cust.sql
      ●	Stored_procedures_dietician_diet.sql
      ●	Stored_procedures_restaurant.sql
      ●	Table_scripts.sql
      ●	Triggers.sql
      ●	Views.sql

      3. Log Directory: Consists of info.txt which has sample log statements.

 
 ******************************  Order of file execution ******************************
 
1. Unzip the cloned folder.
2.	You will get the folder structure as shown in the above source tree
3.	Open SQL directory and run the files in the following order using SQL workbench:
    a.	Table_scripts.sql
    b.	Triggers.sql
    c.	Views.sql
    d.	Stored_procedures_admin.sql
    e.	Stored_procedures_cust.sql
    f.	Stored_procedures_dietician_diet.sql
    g.	Stored_procedures_restaurant.sql
    h.	Insert_Statements.sql

Open mongodb terminal. Create a database “mealmanager” using the command below:
  “use mealmanager;”


4.	Open DB Application Directory and run the files in the following order using visual studio code application:
  a.	Open main.js inside the folder controllers
  b.	Change the user, password at the top of main.js file
  c.	Execute “npm install” command in the terminal of visual studio code
  d.	Execute “node app.js” command in the terminal of visual studio code
  e.	Admin: 
    i.	Open an internet browser and enter the following url: “http://localhost:3000/adminlogin/” to get the admin login page.
    ii.	Enter the following credentials to log in:
      1.	Email ID: admin1@mm.com
      2.	Password: iamadmin1
    iii.	 Once logged in you will be directed to the admin home page where you can perform all the operations listed under admin functionalities in report.
    iv.	Mongo db contact form details can be viewed from contact forms button
  f.	To get the application home page you can enter the following url: “http://localhost:3000/”
  
  g.	Customer:
    i.	To register a new customer you can click on customer registration button.
    ii.	To login with the existing customer, click on the customer login button using and enter the following credentials
      1.	Regular Meal Plan Customer:
        a.	Email ID: Sam@gmail.com
        b.	Password: Sam
      2.	 Dietician Enrolled Customer:
        a.	Email ID: Stephan@gmail.com
        b.	Password: Stephan
    iii.	Once logged in you will be directed to the customer home page where you can perform all the operations listed under customer functionalities in report.
  
  h.	Dietician:
    i.	New dietician can be registered only by admin.
    ii.	To login with the existing dietician  click on the dietician login button and enter the following credentials:
        1.	Email ID: Kate@gmail.com
        2.	Password: Kate
    iii.	Once logged in you will be directed to the dietician home page where you can perform all the operations listed under dietician functionalities in report.
  
  i.	Restaurant:
    i.	New restaurant can be registered only by admin.
    ii.	To login with the existing restaurant click on the restaurant login button and enter the following credentials:
        1.	Email ID: Indian@gmail.com
        2.	Password: Indian
    iii.	Once logged in you will be directed to the restaurant home page where you can perform all the operations listed under restaurant functionalities in report.
  
  j.	Contact Form:
      i.	Click on Contact Form button in the application home page
      ii.	Enter the message and click submit
      iii.	Login to admin page via admin credentials and click on contact messages
      iv.	Previously entered details should be seen

