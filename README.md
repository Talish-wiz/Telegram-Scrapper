# Telegram-Scrapper
Python script that use the Telegram Client API to get all basic usefull data of a group/channel/chat and export them in json files (chat data, members data and messages data).

# How to use
1 - First, you need a Telegram Client-API ID and Application Hash. You can get them by login and creating a new "App" in: https://my.telegram.org

2 - Next, you have to set "API_ID", "API_HASH", "PHONE_NUM" and "CHAT_LINK" (chat that you want to export the data) in "telegram_scrapper.py" file.

3 - Then, you are free to execute "telegram_scrapper.py" file to export the chat data from the "CHAT_LINK" provided: python telegram_scrapper.py

# Points to note
1.The first time that you run the script, it requests a "Sign-in Code", to Telegram client API service, and wait for the user to input that code.

2.The "Sign-in Code" will be sent by "Telegram Service Notifications" account, and it can be read from any Telegram Android/IOS/Desktop App.

3.Once you insert the "Sign-in Code" and the connection is successfully established, the sign-in validation is stored in a file named "Session.session".

4.The "Session.session" file is used in next scripts runs (logins attempts), so it wont request a Sign-in Code again.

5.If you still have problems for sign in when using the correct received code, delete the "Session.session" file and try again.

6.This script must be use from Python 3 (no Python 2 support).

7.The duration of the export process goes from minutes to hours depending on the number of users and messages that the chat has.

