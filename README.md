# Introduction
I'm sick of ubiconnect app so I thought i can make my own GUI app, faster app, not buggy and doesn't collect data to third party.
The result of my research i could find all info about thier rest api using some tools.

I DON'T take any responsibility of the people who intend to harm/spam/abuse ubiconnect or ubisoft via this lib.

# Installation
`pip install jawadpy-ubiconnect`


# Usage
This is really simple and easy to use as it's shown below,

```
import Ubiconnect

ubi = Ubiconnect(YOUR_EMAIL, YOUR_PASSWORD)

# Login to your account
ubi.login() # return json

# get full info about your current account
ubi.current_user_full() # return json

# get small info about your current account
ubi.current_user() # return string

# Sends rest password link to the given email above
ubi.rest_password() # return json

# Get all notifications of the current account
ubi.get_notif() # return json

# Get all games of the current account
ubi.get_games() # return json


## Incase of getting/setting some data:

ubi.getLoginInfo() # return dict

ubi.getUserAgent() # retrun string

ubi.setUserAgent(YOUR_CUSTOM_USER_AGENT_string) # retrun string

# you can set remember me to True/False
ubi.getRememberMe() # return boolen, defualt = False
ubi.setRememberMe(True)


```
