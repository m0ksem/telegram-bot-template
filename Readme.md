# Telegram bot template


## Deploy

### Run as daemon
We use [pm2](https://pm2.keymetrics.io/) that handle background process. This is useful if you have many bot to deploy.

Custom scripts from `./daemon` directory takes process name fron `package.json` so don't forget to change it.

Additional commands:
- `yarn daemon:start` - start new background process
- `yarn daemon:stop` - stop background proces
- `yarn daemon:rebuild` - stop previous process (if exists), build and start new background process

## Requirements 
- Node >16
- yarn >1