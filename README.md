# XKCD challenge
### [Get a COMIC on email in every 5 minutes]

A complete responsive and attractive web application which takes input from user and sends them an email conatining a random xkcd in it.

[![N|Mukul Singh](https://i.ibb.co/VN91CCL/rtcamp.png)](http://demo.techmihirnaik.in/)

## Technologies used:
Entire project is purely created in:

- HTML
- CSS
- PHP
- MYSQL

## Files with brief description:

> **connection.php** : As per the name, this files contains the credentials and creates successful connection to the database.

> **index.php** : Landing page of the project, it conatins the attractive UI where everyone makes a visit. It contains a subscription form responsible for storing user's email-id for every mail functionality. 

> **controller.php** : It conatins the important database operations with security methods (Injection, XCC and other vulnerabilities). It is also responsible for sending verification link via mail.

> **verify-email.php** : This file is mainly resposible for user's email-id verification via a button which user gets in email.

> **xkcd.php** : The mail file of the project , responsible of fetching comics details from xkcd and mails (inline with attachment) them to user's email-id everytime whenever a cron job is executed. Also send a unsubscribe link button in every email.

> **unsubscribe.php** : This file allows user to get unsubscribed on their wish via a button that user's get in mail with comic attachments. On successful unsubscription user's data get deleted from database.

> **resend.php** : It conatins another attractive UI with a form responsible for taking user input and allowing them to request cerification email again.

> **resend-code.php** : This file contains the functionality of resend.php UI that allows user to request verification email again if they haven't received it either due to server time out or any other reason.

**The entire code is created as per PHP coding standards and assignment submission guidelines**
```sh
Demo Link : 
http://demo.techmihirnaik.in/
```
> Created by: `Mukul Singh`
