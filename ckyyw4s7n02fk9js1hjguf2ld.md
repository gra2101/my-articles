## How To Generate A QR Code Using Python

## INTRO
To start with, **QR** in **QR code** is an acronym for **Quick Response**. It is an easy and convenient way to store all kinds of data in a small space. QR code can store over 2000 characters in a small space.

Because of the reason stated above, QR codes are used for many purposes, some of which include:

- **Online accounts authentication: **websites can display a QR code that a registered user can scan with his or her smartphone and automatically log in.
- **Payments:** QR codes can store information about your bank account or credit card.
- **WiFi authentication:** QR codes can be used to keep WiFi networks authentication details such as SSID and password.
- Personal home address, business address, E-mail addresses, and phone numbers can be kept in QR codes.
- URLs of certain web pages or websites can be stored in QR codes.
- QR codes can also be made for verification passkeys used during the configuration of two-step authentication security used by several websites and applications.

## GENERATE A QR CODE WITH PYTHON
With Python, you can generate a QR code with just three lines of code and get it saved on your PC for use. 

> For you to have read to this point, I believe you should have a basic knowledge of Python or any other programming language.

Follow these steps to generate your QR code:

**STEP 1:** 

On your PC, create a folder in any location of your choice and open it with VS code or your preferred code editor.

**STEP 2:** 

Create a Python file in the folder.

**STEP 3:** 

Install the **qrcode** library on your cmd or terminal, using the ```pip install qrcode``` command.

> For you to do this successfully, you must have **python** already installed on your PC alongside **pip**. If you don't, you can get download Python from [here.](https://www.python.org/downloads/)

**STEP 4:** Copy the code below and paste it into your python file.

```
import qrcode
img=qrcode.make("Hello World")
img.save("img.jpg")

```
- The 1st line of the code is calling the ```qrcode``` library to work.
- The 2nd line passes the value **Hello World** that we want our QRcode to have, using the ```qrcode.make()``` function and then assigning it to a variable named **img**. 
- The 3rd line is to save the QR code as an image in our work folder.
 
**PS:** Run the code for the image to save, you should see it in the folder you created earlier that has your python file in it.

## OUTPUT IMAGE

![img.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1643400461029/S6syh14Ew.jpeg)

Use an online QR code scanner to scan the image above and it will display the value we have passed into ```qrcode.make()``` which is **Hello World.** 

Ta-da! We have successfully created a QR code.

## REFERENCE & READ MORE
- [what-are-qr-codes-and-why-are-they-useful/](https://www.digitalcitizen.life/simple-questions-what-are-qr-codes-and-why-are-they-useful/)
- [https://pypi.org/project/qrcode/](https://pypi.org/project/qrcode/)


I hope you have learned from reading this article. 
Do you want to follow me on Twitter? [@graceyomowunmi](https://graceyomowunmi?s=09), or on LinkedIn? [Grace Omowunmi Soyebi](https://linkedin.com/in/gracesoyebi). Ok, bye😉