---
layout: post
title: 'Sending Texts with Python and Twilio'
---
I learned how to manipulate the [Twilio API](https://www.twilio.com/docs/usage/api) in Python to send text messages from my pc's command line.

In my usual style, this was accomplished through many hours of digging through API documentation and YouTube.

I had fun making a small animation for "Sending . . ." at the end.

Here's the code:
```
from twilio.rest import Client
import os
import time

account_sid = os.environ.get('TWILIO_ACCOUNT_SID')
auth_token = os.environ.get('TWILIO_AUTH_TOKEN')
client = Client(account_sid, auth_token)
appTitle = 'SendText, an app by Scott Scharl'
appDescrip = 'Welcome! This app allows you to send a text message to anyone with a US phone number.'
def titleBox():
    print()
    for i in range(len(appTitle)): print('-', end='')
    print('\n' + appTitle)
    for i in range(len(appTitle)): print('-', end='')
    print()
def wait():
    time.sleep(1)

titleBox()
print()
print(appDescrip)
print()
print('Press ENTER to Begin.')
input()

# user inputs where to send the SMS
print("Ok. Let's get started.")
wait()
print()
print("First,")
print("Enter Recipient's Phone Number:")
print('(ten-digit, no spaces, ex: 1234567890)')
to1= input()
wait()
print('...got it, thanks.')
print()
wait()

# adds the country code (+1 for US)
toNumber ='+1' + str(to1)

# user inputs msg text
print('Second,')
print('Enter your message:')
msgBody = input()
wait()
print('...thanks, again!')
print()
wait()

# Confirmation
print("So, to confirm:")
wait()
print()
print('---Your Message---')
print('To: ' + toNumber)
print("Text: " + msgBody)
print('------------------')
print()
time.sleep(3)
print("When you're ready,")
input('Press ENTER to Send.')
print()

# "Sending. . ." animation
waittime = .5
def wait2(waittime):
    import time
    time.sleep(waittime)
def sendDots():
    print('Sending', end='')
    wait2(waittime)
    print("\rSending .", end='')
    wait2(waittime)
    print("\rSending . .", end='')
    wait2(waittime)
    print("\rSending . . .", end='')
    wait2(waittime)
    print("\rSending . . . Sent!")
sendDots()

# Twilio sends the message
message = client.messages \
                .create(
                     body= msgBody,
                     from_= os.environ.get('TWILIO_PHONE_NUM'), # My Twilio number
                     to= toNumber # phone number with added US country code
                 )

# Exit the app
wait()
print()
input('Press ENTER to exit.')
```
