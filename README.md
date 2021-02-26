# HitUp Messenger
A Fully Functioning Chat Messenger (like Whatsapp) built using Flutter.

<img src="https://user-images.githubusercontent.com/47485188/101521998-9c0a2200-39ac-11eb-964a-79d51b4f89c1.png" alt="Screenshot" height="500" width="270"/> <img src="https://user-images.githubusercontent.com/47485188/101522157-dd023680-39ac-11eb-8851-be5b351d3186.png" alt="Screenshot" height="500" width="270"/> <img src="https://user-images.githubusercontent.com/47485188/101532693-e98d8b80-39ba-11eb-804f-78ccad3f1f31.png" alt="Screenshot" height="500" width="270"/>


## About the project
- Flutter for building the Android & IOS App.
- Firestore database for storing user data.
- Firebase Storage for storing images.
- MQTT as messaging protocol hosted in AWS EC2.
- SQLite for storing contacts & chats in Local Database.
- OneSignal for Push Notifications.

## Features

### Phone Number Authentication Sign-in
Authentication is done using Firebase.
<br>

<img src="https://user-images.githubusercontent.com/47485188/101533784-476ea300-39bc-11eb-99b7-4fe09cf2c29a.png" alt="Screenshot" height="500" width="270"/> <img src="https://user-images.githubusercontent.com/47485188/101533474-e0e98500-39bb-11eb-8e67-b50827a8a1e0.png" alt="Screenshot" height="500" width="270"/>


### Sending Images
Send & Receive Messages (Snapchat style UI).
<br><br>
<img src="https://user-images.githubusercontent.com/47485188/101521696-2f8f2300-39ac-11eb-9f42-5afd2ad0e36a.gif" alt="Screenshot" height="500" width="270"/>

### Super Fast Loading of Messages (Using SQLite as Local DB to store messages)

### Sending texts to Phone Contacts
On the Contacts Screen, you will get a list of all your phone contacts who are also using the messenger and can chat with them. (Just like sending messages to your contacts in Whatsapp)<br>

<img src="https://user-images.githubusercontent.com/47485188/101533031-5dc82f00-39bb-11eb-8f53-035e3f01112d.png" alt="Screenshot" height="500" width="270"/>
<br><br>

### Adding contacts using username. Sending & Receiving Friend Requests
You can also send friend request to someone using their username. On sending friend request, the other user will get a push notification & and a friend request. If he/she accepts the request then you will get an notification & will be able to chat with the user. (Same as the feature in Snapchat) <br><br>
<img src="https://user-images.githubusercontent.com/47485188/101530774-5ce1ce00-39b8-11eb-88b5-8d6ae66e049e.png" alt="Screenshot" height="500" width="280"/>

### Block Contact<br>
<img src="https://user-images.githubusercontent.com/47485188/101531982-ea71ed80-39b9-11eb-8d8f-190be70c7131.png" alt="Screenshot" height="500" width="280"/>


### Realtime Push Notifications 
Using OneSignal. User will get realtime push notifications (even when the app is closed) when 
- He/She receives a new message
- He/She receives a friend request
- Someone accepts their friend request

### Super Fast Messaging using MQTT Protocol (MQTT is used by Facebook Messenger)

### Change Profile Photo

### Image Compression Before Sending

### Emoji Support

### Neumorphic UI

### Invite Friends Feature


<br>

## Other Important Information

## Installation & Setup (Optional)
1. Firebase
> To change the firestore database, just replace the google-services.json in android/app to your own google-services.json file from your firebase account.
2. MQTT Server
> To transfer messages I am using an MQTT server which I have setup in a EC2 instance on AWS. For details on how to setup your own MQTT server please refer here : [Setup MQTT Server on AWS EC2](http://blog.yatis.io/install-secure-robust-mosquitto-mqtt-broker-aws-ubuntu/). Then change the serverAddress parameter in lib/functions/MQTTFunction.dart to the public address of your EC2 instance.

file connect() function. <br>

3. OneSignal
> First create an account in [OneSignal](https://onesignal.com/). Then replace the app_id parameter in lib/functions/UserDataFunction.dart sendNotification() function with your own OneSignal app_id.

## Motivation & Contribution
I want to build this messenger into the biggest open source messenger on the web with all functionalities from the top Messengers like Whatsapp, Telegram, Signal, Snapchat, etc. There a lot of features still to be added like end-to-end encryption, audio messages, audio/video calling, stories, etc. So, we are open to pull requests. Please contribute in any way you can, adding new features, finding or fixing bugs, adding to the documenation, better code commenting, etc. 

## Contributing
If you want to contribute to this project other than by coding, please contact me here sdsohan48@gmail.com

## License

