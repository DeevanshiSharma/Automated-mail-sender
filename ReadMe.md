# Automated Birthday mail sending \ python
It is used to automate the process of sends out your birthday wishes to your friends and colleagues via mail.

The basic approach is that the program will check if there's any birthday today from the stored excel sheet and then mail one of the saved letter at random to the birthday person with your wishes in the letter. 

The program uses packages such as Pandas, DateTime, Win10Toast, smtplib, and Random.

Firstly you create an Excel sheet where you store details like name, mail id, and birth date of your friends and colleagues.
Now you have a file that contains all the required data of your birthday mails recipients. So it's time to create some creative birthday wishes for them. Create at least 3 .txt files (birthday letters) and name them as letter_1.txt, letter_2.txt, letter_3.txt, etc and save these files inside the folder letters.

Now for the part of sending out mail:
A function sendEmail() has been defined which will start a Gmail session, send the email, and quit the session. And in the driver code section, the program reads the data from the Excel sheet and matches today’s date with any of the birthdays. If there is a match, sendEmail() function is called. 
Also, ToastNotifier from the win10toast library is used to show desktop notifications once the mail has been sent successfully.

 
