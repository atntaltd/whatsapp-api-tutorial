# Exploring

This branch just for fun!

Let's exploring the whatsapp-web.js library.

## Sending videos or gifs

To make this works, please read this part of the documentation https://guide.wwebjs.dev/features/handling-attachments#sending-media

## If you want to send video or video as sticker on Heroku

For make this works, you must add other buildpacks.

**Send video only**: ```heroku/google-chrome```

**Send video as sticker**: ```heroku/google-chrome``` & ```https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest.git```

Note that you must make the ffmpeg buildpack to the first order. 

And add executablePath option for Puppeteer as shown below.

```js
const client = new Client({
  puppeteer: {
    executablePath: 'google-chrome',
    // ...
});
```
