# XKCD challenge
#### [Get a COMIC on email every 5 minutes]

A complete responsive, attractive, secured and working web application that takes input from users and sends them an email every 5 minutes containing a random xkcd comic in it. Or users can just simply read any random comic online.

[![N|Mukul Singh](https://i.ibb.co/SQSdK5v/rtcamp.png)](http://demo.techmihirnaik.in/)

## Technologies used:
The entire project is purely created in:

- HTML
- CSS
- PHP
- MYSQL

## Description
`Comics is a medium used to express ideas with images, often combined with text or other visual information.`

This web application is designed in such a way as to provides an email every 5 minutes to its subscribers. It asks the user to first input their email-id, If the entered email is valid then a verification mail is sent automatically to their respective mail id.

On successful verification, their email-id is registered in a database with a verified status from where all verified users will receive exclusive comics via mail with an attachment for download. This application also contains a feature to request for re-verification email if by chance any issue they haven't receive any mail at the time of registration.

The mail that every user will receive also contains a unsubscribe button if in case they want a break from receiving regular email.
It's a complete web application with neat/clean and easy to understand code that is fully functioning and has been tested several times to avoid any inconvenience faced by users.

## Files with brief description:

> **connection.php** : As per the name, this file contains the credentials and creates a successful connection to the database.

> **index.php** : The landing page of the project contains an attractive UI where everyone makes a visit. It contains a subscription form responsible for storing the user's email id for every mail functionality.  

> **controller.php** : It contains the important database operations with security methods (Injection, XSS and other vulnerabilities). It is also responsible for sending verification links via mail. 

> **verify-email.php** : This file is mainly responsible for the user's email-id verification via a button which user gets in the email.

> **xkcd.php** : The mail file of the project, responsible for fetching comics details from xkcd and mails  (inline with attachment) to the user's email-id every time whenever a cron job is executed. Also, send a unsubscribe link button in every email.( this file is stored in a non-public directory and cannot be accessed by anyone on server and contains extra layer of security which prevent email script to run by brute-force approach).

> **unsubscribe.php** : This file allows users to get unsubscribed on their wish via a button that user's get in the mail with comic attachments. On successful unsubscription user's data get deleted from the database.

> **resend.php** : It contains another attractive UI with a form responsible for taking user input and allowing them to request re-verification emails again.

> **resend-code.php** : This file contains the functionality of resend.php UI that allows users to request a re-verification email again if they haven't received it either due to server time out or any other reason at the time of registration.

> **view.php** : This file provides the functionality of displaying a random comic every time from where users can view or read any comic online.

**The entire code is created as per PHP coding standards and assignment submission guidelines**
#### Demo Link :
```sh 
http://demo.techmihirnaik.in/

```
> Created by: `Mukul Singh`
