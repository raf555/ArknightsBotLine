# Arknights Bot for LINE
(last update 18-10-2020)

*This is not the real repository for the bot, only for cosmetics for my github account. The real repository is set to private atm.*

## I. Short Introduction
This bot provides you a bunch of information from the game (gacha, recruitment, and operators stuff).

Bot only works on LINE Platform, both personal chat or group/room chat.

## II. The Bot
To add the bot [@563ycerl](https://line.me/R/ti/p/@563ycerl)

# Bot Usage
Send the command (marked one) to the bot


### 1. Recruitment Calculator
Shows you the UI to select the combination.
```sh
recruitment
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Frecruitment%20ui.png?v=1602988225924)
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Frecruitment%20info.png?v=1602988225924)
### 2. Gacha Simulator
Both event and standard banners follow the current banners in EN server.
### 2.1. To select banner:
```sh
gacha select
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Fgacha%20select.png?v=1602988391923)
### 2.2. To do the gacha (x = total pulls):
```sh
gacha x
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Fgacha.png?v=1602988391654)
*this result was shown only for testing, doesn't represent neither the system nor my luck*

### 2.3. To see gacha result statistic:
```sh
gacha stat
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Fgacha%20stat.png?v=1602988390869)
### 2.4. To reset the statistic:
```sh
gacha reset
```
### 3. Operators Information
Operators information follow the latest game update (CN server)

*credit to Gamepress for this*

x = Operator's name.
```sh
info x
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2F832319.jpg?v=1602991181436)
### 3.1. Operators Material Information
x = Operator's name
```sh
mats x
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Fmats.png?v=1602990117363)
### 3.2. Operators Stats Information
x = Operator's name
```sh
stats x
```
![](https://cdn.glitch.com/2b183aba-b05a-49d5-a693-0660debb54c6%2Fstats.png?v=1602990117412)
### 4. Materials Craft Recipe
Can only be accessed from *mats x* command.

*click the materials*

![](https://im.ezgif.com/tmp/ezgif-1-6f6461e49e33.gif)


## III. Error Reply
If something happen to the features, bot will send you message like this.

![](https://image.prntscr.com/image/KKHdRa-xSuCLOqjXzcD6qg.png)

This is mostly caused by
1. Bot process the command more than 30 seconds
2. Outdated database

### First Issue
For the first cause, it is mostly happened when bot is waking up, you may notice this by telling how long does the bot reply.
LINE limits the reply time for less than 30 seconds, so this happens. For this issue, when you resend the message, it should be work just fine after that.

### Second Issue
For the second cause, it is simply caused by outdated database (such as mats and stats features), it will give you the same message, 
but when you resend the message, it will give you the same message again, i anticipated this by adding report system, so when error happens for several times,
you will see report button and the features will be disabled temporarily and the report will be sent to me.

## IV. Features that are probably added in the future
1. ~Group / Room support.~ added.

## V. Bot Specification and Source Code
Because of scrappy and not structured code atm, i have no plan to release the code, it is embarassing, lol.

Bot is using NodeJS for the system and simple JSON data application for the database and currently using free hosting service from [Glitch](https://glitch.com).

![](https://image.prntscr.com/image/JG9UOTz1RaK0F1tESk2uag.png)

Database editing for gacha is using simple front end application.

![](https://image.prntscr.com/image/--jGuyFtRmeeNrPSsE26vg.png)
