# Smart-Door-Bell

This system is for security purposes, Ultrasonic sensor, webcam, buzzer(doorbell), telegram has been associated within.
What it will do is when you wave your hand over ultrasonic sensor, It will send a picture to telegram bot or any other social media platform using webcam and triggers the buzzer demonstrating as a doorbell. This process can continue till you want.

Materials:-

1)Raspberry Pi 3

2)Ultrasonic Sensor

3)Usb WebCam

4)Jumper Wires

5)BreadBoard

6)Buzzer

Circuit:-

(UltraSonic Sensor)

Vcc - 5v

Echo - GPIO23

Trig - GPIO18

Gnd - Ground

Buzzer(Red wire) - GPIO24

Buzzer(Black wire) - Ground

Important :-

1)Create your own bot . If you don't know how to create one refer to the link below:- https://www.instructables.com/id/Set-up-Telegram-Bot-on-Raspberry-Pi/

2)Know your chat id :- 1.Open Telegram app and search "get id" or "@get_id_bot"

                       2.Type "/start" , You will get your chat id
                   
                       3.You can also refer to the video below :-
                         https://www.youtube.com/watch?v=2jdsvSKVXNs
Things to change in the code :-

1)(See Line 50 and 51) Change from the chat-id in the code to your chat-id .

telegram_bot.sendMessage (Chat_id, message)

telegram_bot.sendPhoto(Chat_id,photo=open("imagetest.jpg"))

2)(See line 58) Change from the default_token to your token

telegram_bot = telepot.Bot('default_token')

How to run .py file in Raspberry pi?

1)Open terminal

2)Go to the .py file location

3)Type python file_name.py

That's all.
