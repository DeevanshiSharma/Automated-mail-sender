# Automated Birthday mail sender\ python
 Automated birthday mail sender automatically sends out your personalised mails to your friends and colleagues vie your mail id.

The basic idea behind this code is that the program will check if there's any birthday today from the stored excel sheet and then mail one of the saved letter to the birthday person with your personalized wishes in the letter. 

The program uses 6 main libraries:

-Pandas

-dateTime

-smtplib

-time

-random

-win10toast

Now to begin setup you need to create an excel sheet with records like Name, Email and, Birthday of your friends and colleagues to whom you want to send birthday mails.

Now you have a file that contains all the required data of your birthday mails recipients. So it is time to create some creative birthday messages for them. Create at least 3 .txt files (birthday letters) and name them as letter_1.txt, letter_2.txt, letter_3.txt, etc and save these files inside the folder letters.

The basic approach of this program is:

For the sending email part, a function sendEmail() has been defined which will start a Gmail session, send the email, and quit the session. And in the driver code section, the program reads the data from the Excel sheet and matches today’s date with any of the birthdays. If there is a match, sendEmail() function is called. Also, ToastNotifier from the win10toast library is used to show desktop notifications once the e-mail has been sent successfully.

 
