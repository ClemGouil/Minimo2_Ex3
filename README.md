# Minimo2_Ex3
Here my work for the minimo 2 ! I had exercise 3 !

Here you have the Android part, to achieve this part, I created a MessageInboxActivity activity with its respective layout activity_message_inbox.xml. I also created my model a Message class which contains a String message attribute.

In the UserService interface I added the getMessages() function which, thanks to retrofit, calls the API and returns the json of all the messages to us. (I also changed the address of the API which was of the EETAC machine into that of the local machine).

In the new layout, I therefore put a recycleview in order to display all the subsequent messages that are obtained following the HTTP request.

In the new activity created, I have therefore defined an adapter for the recycleview to adapt to the json file that we will retrieve when calling getMessages().

In the other directory where there is the backend, I defined my "dummy" function GetMessages which returns me a list of messages and if we test this activity we see that everything works, the messages are displayed correctly.
In the Backend, I removed all the part that used the database because it was bugging everything.

I added link my new activity to the forum button of the main activity.
