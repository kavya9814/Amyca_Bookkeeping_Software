###How to run Amyca bookkeeping software web application

This project is based on django framework with all the HTML(UI of the project)files will be availble in template folder.
All the pictures and necessary styling files will be available in the static folder.

###Scripts

All the python scripts will be available in the project folder.


Make sure to have latest python version installed(preferbly version above 3.5)
https://www.python.org/downloads/

Install XAMPP control panel
https://www.apachefriends.org/download.html
#### start the XAMPP control panel

Open the XAMPP control panel and start the services Apache and MySQL as shown below

![Referenceimage](/xampp.JPG)

### run the code

1) Open cmd in the project folder
![Referenceimage](/pic1.JPG)

2)  Follow the below steps 

![Referenceimage](/pic2.JPG)

This will give the IP address of the development server.

3) Use the IP address to access the UI of the project
![Referenceimage](/pic3.JPG)


##### add from_mail for OTP generation in forgot password
forgot password changes

If you want to add new from email address to this feature 
1) Enable two step verification in security for the account
2) Use below link to create app password
https://myaccount.google.com/apppasswords?utm_source=google-account&utm_medium=web

Select app -> custom ->name it as amyca 
Copy the 16 digit selected password
3)Go to forgotpassword -> views.py 
change frommail in __sendmail method to your new email address
In PWD add the 16 digit password generated 
4) Replace the client ID in l16 line in subscritpions_plans.html file to change the paypal receiver client Id
5) restart the server 



