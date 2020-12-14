# Whatsapp API Tutorial

Hi, this is the implementation example of <a href="https://github.com/pedroslopez/whatsapp-web.js">whatsapp-web.js</a>

Watch the tutorials:
- <a href="https://youtu.be/IRRiN2ZQDc8">Whatsapp API Tutorial: Part 1</a>
- <a href="https://youtu.be/hYpRQ_FE1JI">Whatsapp API Tutorial: Part 2</a>
- <a href="https://youtu.be/uBu7Zfba1zA">Whatsapp API Tutorial: Tips & Tricks</a>
- <a href="https://youtu.be/ksVBXF-6Jtc">Whatsapp API Tutorial: Sending Media File</a>
- <a href="https://youtu.be/uSzjbuaHexk">Whatsapp API Tutorial: Deploy to Heroku</a>
- <a href="https://youtu.be/5VfM9PvrYcE">Whatsapp API Tutorial: Multiple Device</a>
- <a href="https://youtu.be/Cq8ru8iKAVk">Whatsapp API Tutorial: Multiple Device | Part 2</a>

### How to use?
- Clone or download this repo
- Enter to the project directory
- Run `npm install`
- Run `npm run start`
- Open browser and go to address `http://localhost:8000`
- Scan the QR Code
- Enjoy!

### Notes
As mentioned in the video above, you have to install `nodemon` to run the start script. You can install nodemon globally with `npm i -g nodemon` command.

### Send message to group
I was added an example to send a message to groups, but before that we must know the group ID (chat ID). Don't worry, I also add the functionality to help you to get that groups ID.

Here the way to get the groups info (including ID & name):
- Send a message to the API number `!groups`
- The API will replying with the groups info
- Use the ID to send a message
- Here the endpoint: `/send-group-message`