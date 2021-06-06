## PTNK Chatible

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

#### Chatible clone written in TypeScript, based on Node, Express and Mongo

Demo: https://m.me/ptnkchat

## Basic instruction

- Deploy to Heroku using the deploy button.
- Create a cluster on MongoDB Atlas. Whitelist IP addresses.
- Create an app on Facebook. Install Webhook. Get app secret and tokens.
- Set Heroku's `Config Vars`. Check [here](src/config/index.ts) to know which variables you need to set.

### Essential `Config Vars`: 

1. Facebook app properties:
- APP_SECRET
- PAGE_ACCESS_TOKEN
- PAGE_VERIFY_TOKEN (You can define at your choice)
- APP_NAME (must be the same on Heroku, and this name will appear on bot's introduction)
- DEV_ID (Facebook App's ID)
2. MongoDB:
- MONGO_URI
3. Customized Icon:
- PERSONA_PROFILE_PICTURE (recommended)
4. Others:
- ADMIN_PASSWORD
- HEROKU_API_KEY
    
### Enjoy!!!


## Features

- Admin dashboard ([code](https://github.com/ptnkchat/ptnkchat.github.io))
- Pair by gender (e.g. male with female)
- Send cute dog/cat pictures
- Customizable message templates
- Cache database in memory to increase performance
- Developed with performance in mind
- Already matched people will not meet again

## Planned features

- Allow editing profile via Messenger Webview
- Limiting rate of requests sent out to avoid being converted to [high-MPS](https://developers.facebook.com/docs/messenger-platform/send-messages/high-mps) page

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Credit

- Nguyen Xuan Son (a.k.a Nui or [@ngxson](https://github.com/ngxson)) for [Chatbot CHN](https://github.com/ngxson/chatbot-cnh) on which this project was originally based
- Le Bao Hiep ([@hieplpvip](https://github.com/hieplpvip)) for maintaining this project
