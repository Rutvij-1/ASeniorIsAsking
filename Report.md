# ASeniorIsAsking

It's past midnight. You're hungry. You're grumpy. You want nothing but food. But... you're lazy too. What would you not do for a Tawa Bonda or a Shawarma? If only you knew which fachcha is already out there at DLF... Inspired from the 3am chats on the UG2k19 WhatsApp Groups, we present to you the only app you'll ever need to fulfill your heart's desire of having that one last meal before your regular 3-hour sleep.

<img src="./readme_media/BaseImageGIF.gif" height="450" align="center"/>

### Backend

This is a Flask app. It functions on a Redis Server and uses API calls to send and recieve data. The functions of the following files are such:

* [app.py](backend/src/app.py) - This file starts the app on the server.
* [config.py](backend/src/config.py) - This file contains the information about the redis server.
* [model.py](backend/src/model.py) - This file contains the redis connection class which stores the data coming from frontend, retrieves and performs functions on the data stored in the database.
* [views.py](backend/src/views.py) - This file contains the API call routes through which the front end web pages can connect to the Redis database.

## Future Plans

Since this app was built under time pressure, we were able to add limited features and support. But given more time and resources here are some of the improvements we would make to this app:

* We would set this app on a cloud based server, or if possible IIIT server.
* We would add CAS authentication to restrict this app for IIIT use only.
* We would make an android and ios app to make it easier for people to order and accept orders.

## Other Potential Uses

The technology behind this app can be used for other purposes too. Some of them are:

1. You live in a city and you need groceries, but a lockdown is in effect. You would like to avoid leaving your home whenever possible, like a responsible citizen.<br>A lot of people live in your neighbourhood because, well you live in a city. So why not ask someone to get your groceries for you?<br>But how would you know who is out buying groceries and who is enjoying their afternoon nap?<br>This is where this app can come in. You just post a request for whatever groceries you need urgently, and anyone who already is out of their home or is planning to go out soon can get you your groceries.<br>You as a young and healthy person may not understand the importance of this app. But now imagine you are an old person living alone. You are already scared because Covid-19 is fatal for you, and now you don't have food to eat. This app can relieve you of a lot of your problems.
