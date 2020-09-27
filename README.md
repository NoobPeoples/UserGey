<p align="center">
    <a href="https://github.com/X-Newbie/X-Userge">
        <img src="resources/userge.png" alt="X-Userge">
    </a>
    <br>
    <b>Pluggable Telegram UserBot</b>
    <br>
    <a href="https://github.com/X-Newbie/X-Userge#inspiration-">Inspiration</a>
    &nbsp•&nbsp
    <a href="https://github.com/X-Newbie/X-Userge#features-">Features</a>
    &nbsp•&nbsp
    <a href="https://github.com/X-Newbie/X-Userge#example-plugin-">Example</a>
    &nbsp•&nbsp
    <a href="https://github.com/X-Newbie/X-Userge#requirements-">Requirements</a>
    &nbsp•&nbsp
    <a href="https://github.com/X-Newbie/X-Userge#project-credits-">Project Credits</a>
    &nbsp•&nbsp
    <a href="https://github.com/X-Newbie/X-Userge#copyright--license-">Copyright & License</a>
</p>

<p align="center"><b>🔥 X-Userge 🔥</b></p>

[![Build Status](https://travis-ci.com/UsergeTeam/Userge.svg?branch=dev)](https://travis-ci.com/UsergeTeam/Userge) ![Python Version](https://img.shields.io/badge/python-3.8-lightgrey) ![Release](https://img.shields.io/github/v/release/UsergeTeam/Userge) ![Stars](https://img.shields.io/github/stars/UsergeTeam/Userge) ![Forks](https://img.shields.io/github/forks/UsergeTeam/Userge) ![Issues Open](https://img.shields.io/github/issues/UsergeTeam/Userge) ![Issues Closed](https://img.shields.io/github/issues-closed/UsergeTeam/Userge) ![PR Open](https://img.shields.io/github/issues-pr/UsergeTeam/Userge) ![PR Closed](https://img.shields.io/github/issues-pr-closed/UsergeTeam/Userge) ![Contributors](https://img.shields.io/github/contributors/UsergeTeam/Userge) ![Repo Size](https://img.shields.io/github/repo-size/UsergeTeam/Userge) ![License](https://img.shields.io/github/license/UsergeTeam/Userge) ![Commit Activity](https://img.shields.io/github/commit-activity/m/UsergeTeam/Userge) [![Plugins Repo!](https://img.shields.io/badge/Plugins%20Repo-!-orange)](https://github.com/UsergeTeam/Userge-Plugins) [![Join Channel!](https://img.shields.io/badge/Join%20Channel-!-red)](https://t.me/theUserge) [![DeepSource](https://static.deepsource.io/deepsource-badge-light-mini.svg)](https://deepsource.io/gh/UsergeTeam/Userge/?ref=repository-badge)

> **X-Userge** is a Powerful , _Pluggable_ Telegram UserBot written in _Python_ using [Pyrogram](https://github.com/pyrogram/pyrogram).

## ORIGINAL REPO BY

* [USRGE TEAM](https://github.com/UsergeTeam/Userge)

## Inspiration 😇

> This project is inspired by the following projects :)

* [tg_userbot](https://github.com/watzon/tg_userbot) ( heavily ) 🤗
* [PyroGramUserBot](https://github.com/SpEcHiDe/PyroGramUserBot)
* [Telegram-Paperplane](https://github.com/RaphielGang/Telegram-Paperplane)
* [UniBorg](https://github.com/SpEcHiDe/UniBorg)

> Special Thanks to all of you !!!.

<details>
  <summary>Features 😍 </summary>

* Powerful and Very Useful **built-in** Plugins
  * gdrive [ upload / download / etc ] ( Team Drives Supported! ) 🤥
  * zip / tar / unzip / untar / unrar
  * telegram upload / download
  * pmpermit / afk
  * notes / filters
  * split / combine
  * gadmin
  * plugin manager
  * etc...
* Channel & Group log support
* Database support
* Build-in help support
* Easy to Setup & Use
* Easy to add / port Plugins
* Easy to write modules with the modified client

</details>

## Example Plugin 🤨

```python
from userge import userge, Message

LOG = userge.getLogger(__name__)  # logger object

CHANNEL = userge.getCLogger(__name__)  # channel logger object

@userge.on_cmd("test", about="help text to this command")  # adding handler and help text to .test command
async def testing(message: Message):
   LOG.info("starting test command...")  # log to console

   await message.edit("testing...", del_in=5)  # this will be automatically deleted after 5 sec

   await CHANNEL.log("testing completed!")  # log to channel
```

## Requirements 

* Python 3.8 or Higher 👻
* Telegram [API Keys](https://my.telegram.org/apps)
* Google Drive [API Keys](https://console.developers.google.com/)
* MongoDB [Database URL](https://cloud.mongodb.com/)

<details>
  <summary> How To Deploy 👷 </summary>

```
* **[HEROKU](https://www.heroku.com/) Method** 🔧

  > First click the button below. 

  > If you don't have HU_STRING_SESSION just ignore it.  

  > After Deployed to Heroku first turn off the app (resources -> turn off) and run `bash genStr` in console (more -> run console).  

  > After that copy the string session and past it in Config Vars (settings -> reveal config vars). 

  > Finally turn on the app and check the logs (settings -> view logs) :)
```

<p align="center">JOIN CHANNEL TO GET DEPLOY BUTTON</p>
<p align="center"><a href="https://t.me/XBOT_SUPPORT">   <img src="https://img.shields.io/badge/JOIN%20CHANNEL-blueviolet?style=flat&logo" width="210" height="34.45" /></a>
<br>
</p>

</details>

<details>
  <summary> Other Method** 🔧 </summary>

  ```bash
  # clone the repo
  git clone https://github.com/X-Newbie/X-Userge.git
  cd X-Userge

  # create virtualenv
  virtualenv -p /usr/bin/python3 venv
  . ./venv/bin/activate

  # install requirements
  pip install -r requirements.txt

  # Create config.env as given config.env.sample and fill that
  cp config.env.sample config.env

  # get string session and add it to config.env
  bash genStr

  # finally run the Userge ;)
  bash run
  ```
</details>

* **[More Detailed Guide](https://docs.google.com/document/d/15uoiOn2NkN518MMkx9h5UaMEWMp8aNZqJocXvS0uI6E)** 📝

> TODO: add Docker Support.

## Generate String Session
Easy way to generate string session on Repl.it:

<p align="center"><a href="https://GenUserGeString.usergeuserbot.repl.run"> <img src="https://telegra.ph/file/7193be9fb5f9caa50bae8.png" alt="Generate String Session" /></a></p>


### Video Tutorial 🎥

  [![Tutorial](resources/tutorial.jpg)](https://youtu.be/M4T_BJvFqkc "Tutorial")

### Support & Discussions 👥

> Head over to the [Discussion Group](https://t.me/slbotsbugs) and [Update Channel](https://t.me/theUserge)

### Project Credits 💆‍♂️

* [Specially to these projects](https://github.com/UsergeTeam/Userge#inspiration-) 🥰
* [@uaudIth](https://t.me/uaudIth)
* [@K_E_N_W_A_Y](https://t.me/K_E_N_W_A_Y)
* [@nawwasl](https://t.me/nawwasl)
* [@TharukaN97](https://t.me/TharukaN97)
* [@Supun97](https://t.me/Supun97)
* [@gotstc](https://t.me/gotstc)

### Copyright & License 👮

* Copyright (C) 2020 by [UsergeTeam](https://github.com/UsergeTeam) ❤️️
* Licensed under the terms of the [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/UsergeTeam/Userge/blob/master/LICENSE)
