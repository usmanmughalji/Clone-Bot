# Gdrive files/folders Clone Bot
This is a telegram bot writen in python for cloning files/folders to our beloved Google Drive.


[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/)
<a href="https://www.python.org/"><img alt="language" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg"/></a>
[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)


# Inspiration 
This project is heavily inspired from @Izzy12's telegram bot.

# Features supported:
- Clone Gdrive Files and Folders
- Docker support
- Uploading To Team Drives.
- Index Link support
- Service account support


# How to deploy in Heroku?
Hit the deploy to heroku button and follow the further instructions in the screen:


[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/death-angel-141/Clone-Bot.git)


 

## Getting Google OAuth API credential or SECRET_JSON

- Visit the [Google Cloud Console](https://console.developers.google.com/apis/credentials)
- Go to the OAuth Consent tab, fill it, and save.
- Go to the Credentials tab and click Create Credentials -> OAuth Client ID
- Choose TV and Limited Input Devices and Create.
- Visit [Google API page](https://console.developers.google.com/apis/library)
- Search for Drive and enable it if it is disabled
- Finally, run the script to generate SECRET_JSON for Google Drive

```
pip install oauth2client
```
```
python3 generate_drive_token.py
```
OR use online terminal

[![Run on Repl.it](https://repl.it/badge/github/death-angel-141/String-Session-Generator)](https://CraftySeagreenMethod.loda6969.repl.run)

**Termux:**

``` pkg install python wget ```

``` wget https://raw.githubusercontent.com/CW4RR10R/python-aria-mirror-bot/master/generate_drive_token.py ```

``` pip install oauth2client ```

``` python3 generate_drive_token.py ```
___


Fill up rest of the fields in app.json. Meaning of each fields are discussed below:
- **BOT_TOKEN** : The telegram bot token that you get from @BotFather
- **GDRIVE_FOLDER_ID** : This is the folder ID of the Google Drive Folder to which you want to upload all the mirrors.
- **DOWNLOAD_DIR** : The path to the local folder where the downloads should be downloaded to
- **DOWNLOAD_STATUS_UPDATE_INTERVAL** : A short interval of time in seconds after which the Mirror progress message is updated. (I recommend to keep it 5 seconds at least)  
- **OWNER_ID** : The Telegram user ID (not username) of the owner of the bot
- **AUTO_DELETE_MESSAGE_DURATION** : Interval of time (in seconds), after which the bot deletes it's message (and command message) which is expected to be viewed instantly. Note: Set to -1 to never automatically delete messages
- **IS_TEAM_DRIVE** : (Optional field) Set to "True" if GDRIVE_FOLDER_ID is from a Team Drive else False or Leave it empty.
- **USE_SERVICE_ACCOUNTS**: (Optional field) (Leave empty if unsure) Whether to use service accounts or not. For this to work see  "Using service accounts" section below.
- **INDEX_URL** : (Optional field) Refer to https://github.com/maple3142/GDIndex/ The URL should not have any trailing '/'
- **API_ID** : This is to authenticate to your telegram account for downloading Telegram files. You can get this from https://my.telegram.org DO NOT put this in quotes.
- **API_HASH** : This is to authenticate to your telegram account for downloading Telegram files. You can get this from https://my.telegram.org
- **SESSION_STRING** : Session string generated by running:

```
pip install pyrogram tgcrypto
```
```
python3 generate_string_session.py
```
OR use online terminal

[![Run on Repl.it](https://repl.it/badge/github/death-angel-141/String-Session-Generator)](https://HastyCornsilkRecovery.loda6969.repl.run) 

**Termux:**

``` pkg install python wget ``` (if not installed earlier)

``` wget https://raw.githubusercontent.com/CW4RR10R/python-aria-mirror-bot/master/generate_string_session.py ```

``` pip install pyrogram tgcrypto ```

``` python3 generate_string_session.py ```

___

 

