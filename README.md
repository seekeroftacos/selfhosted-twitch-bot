# Contributing to this project

- To contribute, all you have to do is:

> Clone this repo

> Push and commit your changes

- After this is done, please be patient as I do not frequently check this repo.
  - If you do not get a response back about your PR within 48 hours, feel free to contact me on Discord @ `Asqry#1234`

### Quality of code contributed:

- I'm not gonna be the code quality nazi, all I ask is that you make it clean-ish and easy to read (variable, function, and file names)
- This project uses the TMI.js library to connect to the Twitch IRC, the TMI.js docs are located [here](https://github.com/tmijs/docs/tree/gh-pages/_posts/v1.4.2)
  \
  \
  \
  \
  &nbsp;

# Self-hosting this project

- Hosting this project yourself is super simple! Just follow these instructions and you should have your very own bot running in no time!

## Setup Steps:

&nbsp;

### Installing Node.js

- Install the latest version of Node.js here:
  - [Windows](https://nodejs.org/dist/v14.16.0/node-v14.16.0-x64.msi)
  - [MacOS (.pkg)](https://nodejs.org/dist/v14.16.0/node-v14.16.0.pkg)
  - [Linux (Source Code)](https://nodejs.org/dist/v14.16.0/node-v14.16.0.tar.gz)

&nbsp;

### Cloning this repository

- Download the repo in .zip form [here](https://github.com/seekeroftacos/selfhosted-twitch-bot/archive/main.zip)
- Locate the download location, and extract the downloaded files

&nbsp;

### Installing npm libraries

- Locate the folder you just extracted
- Open it in your favorite terminal application
- Verify that the `package-lock.json` file exists
- Run the command `npm install`
  - NPM errors? Run the command `npm audit fix`
  - If that doesn't work, feel free to contact me on Discord @ `Asqry#1234`

&nbsp;

### Configuring your environment variables

- This project utilizes environment variables to store important information and constants

  - For your safety, do not share any of the contents of this file with anyone.

- Create a file in your folder called `.env`
- Copy the contents of `.env.example` into your new `.env` file

- Replace the `ACTIVE_CHANNEL` variable with your Twitch username
- Replace the `BOT_USERNAME` variable with your bot account's username
- Replace the `COLOR` variable with the color you want your bot to use in chat
  > ```js
  > colors = [
  >   'Blue',
  >   'BlueViolet',
  >   'CadetBlue',
  >   'Chocolate',
  >   'Coral',
  >   'DodgerBlue',
  >   'Firebrick',
  >   'GoldenRod',
  >   'Green',
  >   'HotPink',
  >   'OrangeRed',
  >   'Red',
  >   'SeaGreen',
  >   'SpringGreen',
  >   'YellowGreen',
  > ];
  > ```
  - If your bot account has Twitch prime, you can use any [hex code](https://www.color-hex.com/) as your bot's color
- Replace the `OAUTH_TOKEN` variable with a token retrieved from [https://twitchapps.com/tmi](https://twitchapps.com/tmi)
- Replace the `CLIENT_ID` variable with your Client ID
  - Generating a Client ID:
    - Head to https://twitchtokengenerator.com
    - When prompted, press "Custom Scope Token"
    - Find the `CLIENT ID` field, and press "Copy" to copy your Client ID
- Replace the `TOKEN` variable with your access token
  - Generating your scope token:
    - On the same page as your Client ID:
      - Scroll down, and press "Generate Token!"
        - Authorize with Twitch
      - Solve the captcha
      - Verify that the account name listed at the top of the page is correct
      - Find the `ACCESS TOKEN` field, and press "Copy" to copy your access token
