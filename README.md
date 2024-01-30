# Find Phone through Home Assistant

## Prerequisites
- User entities (person.username) that can be tracked and identified as Home or Away (or in other zones).
- User phones with the Home Assistant App that can recieve notificaitons
- A way to receive a notification and respond to it
  - In this example, I have Alexa Media Player and Alexa Actionable Notifications set up to send notifications 
via a skill and recieve a response.
  - You can edit the code to use Assist, popups on a home dashboard, an actionable notification to another
users phone, etc.
  - You can also skip having a response and simply not allow the critical alert to go through when the user
is in certain zones.

## Set-up
- Add the input_booleans to your config.yaml or create them through the Helpers UI, creating one for each user.
- Paste the first automation into a new automation. Update the trigger entities to your new input_boolean and the variable to your user details. Edit the action > choose > default as needed.
- Paste the second automation into a new automation. Again, updated the trigger and user details. Depending on your "phone not at home" notifcation mode, you may be able to add the response code to the first automation and continue using the variables.
- Paste teh third automation into a new automation and update the trigger and turn off entitites.
- [Add the custom sound]([https://github.com/keatontaylor/alexa-actions/wiki](https://companion.home-assistant.io/docs/notifications/notification-sounds/#:~:text=In%20the%20Home%20Assistant%20companion,sounds%20you%20wish%20to%20add.)https://companion.home-assistant.io/docs/notifications/notification-sounds/#:~:text=In%20the%20Home%20Assistant%20companion,sounds%20you%20wish%20to%20add.) to your phone's notification. 

