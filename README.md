

```

```

Note that you need to configure a reverse proxy if you need HTTPS.

### Host bare-metal with Node.js

Install Node.js 14.x, then:

```
git clone https://github.com/soruly/trace.moe-telegram-bot.git
cd trace.moe-telegram-bot
npm install
```

- Copy `.env.example` to `.env`
- Edit `.env` as you need

```
node server.js
```

### Host bare-metal with pm2

You also can use [pm2](https://pm2.keymetrics.io/) to run this in background in cluster mode.

Use below commands to start / restart / stop server.

```
npm run start
npm run stop
npm run reload
npm run restart
npm run delete
```

To change the number of nodejs instances, edit ecosystem.config.json
