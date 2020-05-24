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
* When made as an app that can be deployed on a smart phone, we would add a smart notification system that notifies the person who is near a stall about the food orders placed from that stall.<br>For example, if one person ordered shawarma then the app notifies all the IIIT people near any shawarma stall.

## Other Potential Uses

The technology behind this app can be used for other purposes too. Some of them are:

1. You live in a city and you need groceries, but a lockdown is in effect. You would like to avoid leaving your home whenever possible, like a responsible citizen.<br>A lot of people live in your neighbourhood because, well you live in a city. So why not ask someone to get your groceries for you?<br>But how would you know who is out buying groceries and who is enjoying their afternoon nap?<br>This is where this app can come in. You just post a request for whatever groceries you need urgently, and anyone who already is out of their home or is planning to go out soon can get you your groceries.
2. A similar app can be deployed in seperate hostels for the super lazy or super sick people to get food from in-campus vendors.
3. All the cities in India are flooding with traffic. This has led to increase commute times and icnreased carbon emissions.<br>Public transport is a solution, but it doesn't take you everywhere. So if your office is in the outskirts of the city, you are forced to use your personal vehicle.<br>But there is a solution, and it is known as "carpool".<br>Now imagine that you don't have a car and it's your first day at work, and you don't know anyone. What do you do?<br>To solve this problem, a company can set up this app where some people who are not in a carpool can post requests, and anyone driving nearby to them can offer them a lift and accept their requests and drive them to work.
