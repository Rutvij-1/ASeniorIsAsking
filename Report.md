# ASeniorIsAsking
 
It's past midnight. You're hungry. You're grumpy. You want nothing but food. But... you're lazy too. What would you not do for a Tawa Bonda or a Shawarma? If only you knew which fachcha is already out there at DLF... Inspired from the 3am chats on the UG2k19 WhatsApp Groups, we present to you the only app you'll ever need to fulfill your heart's desire of having that one last meal before your regular 3-hour sleep.
 
<img src="./readme_media/BaseImageGIF.gif" height="450" align="center"/>
 
### Backend
 
This is a Flask app. It functions on a Redis Server and uses API calls to send and recieve data. The functions of the following files are such:
 
* [app.py](backend/src/app.py) - This file starts the app on the server.
* [config.py](backend/src/config.py) - This file contains the information about the redis server.
* [model.py](backend/src/model.py) - This file contains the redis connection class which stores the data coming from the frontend, retrieves and performs functions on the data stored in the database.
	* __init__ - Initializes the object of the class and creates a connection to the Redis Server.
	* inc_count - This function increases the value that maintains the number of orders received.
	* get_count - This function returns the value that maintains the number of orders received.
	* valid_order - This function indicates whether the passed order id is linked to a valid order or not.
	* pending_order_add - This function adds the order data that it receives from the front end, links it to a newly generated order id and returns that order id.
	* get_particular_pending - It returns the order data linked to the passed order id if that order is not accepted or not deleted.
	* get_all_pending - It returns the python dictionary that contains the data of all the pending orders stored in the Redis database.
	* get_particular_done - It returns the order data linked to the passed order id if that order has been accepted.
	* get_all_pending - It returns the python dictionary that contains the data of all the accepted orders stored in the Redis database.
	* has_it_been_accepted - It indicates whether the order linked to the passed order id has been accepted or not.
* [views.py](backend/src/views.py) - This file contains the API call routes through which the front end web pages can connect to the Redis database.
