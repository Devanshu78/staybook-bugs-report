# StayBook

## Task: Booking Flow Bug & UX Audit

### 1) Chat Bot

- Nowadays, people use GenAI chatbots; yours feels too robotic.

<!-- ![Chat box screenshot](./images/image.png) -->

- Suggestions
  - "Plan Your Trip with Us?" should be a statement, not a question.
  - You can change the profile picture and give the chatbot a beautiful name.
  - Try to add a GenAI solution to make it more human-like and engaging to interact with.

### 2) Spacing at eVisa Section

- Spacing can be improved.
- The price in dollars and INR should be bold, and you can use the INR icon as a tag.
<!-- ![spacing at eVisa page](./images/image1.png) -->

- No one is going to read all this; they will just do as shown in the video.

<!-- <video controls src="./images/20250707-1550-16.1426639.mp4" title="Long Text"></video> -->

- Solution
  - You can categorize the text data and fit it into a smaller area so that users don't have to scroll as much.
  - You should implement this even if the user doesn't search for anything.
  - You should also change the spacing and font to make it look better.

<!-- ![Category option which is available by default](./images/image2.png) -->

- When we select any country, the image you are loading takes more time, which makes your website slow.
  - You can upload all the assets to Cloudinary or any platform that gives you a public access link for each image, and store all those URLs in a Redis cache so that users don't feel any lag.

### 3) Network Logs

<!-- ![Browser Network Section](./images/image3.png) -->

- Check this network log to see how many requests it makes to the server.
- If you see something named _collect_ which makes requests again and again, it just increases your bandwidth cost. It looks like you are polling, but this can be avoided by using a WebSocket.
- There are many more requests that you can avoid by using SVGs for your logo, dropdown, social media icons, and many more.

### 4) Login problem

<!-- ![Login Problem](./images/image4.png) -->

- If a user enters the wrong password, why is there text in the password field? They have to delete the text first, which makes the experience bad.

### 5) Hotel loading Skelton

<!-- ![alt text](./images/image5.png) -->

- It looks too hard and has sharp edges. You can make them a little more rounded to give a premium feel.

### 6) Filters

<!-- ![alt text](./images/image6.png) -->

- When users apply filters, they stack up in a very small space and ruin the experience. You can redesign this so that it doesn't bother them.

### Responivenes

<!-- ![alt text](./images/image7.png) -->

- In the tablet section, the UI feels a bit odd as it does not have padding on the left and right.
- It's too cluttered, which does not follow design principles that emphasize the importance of spacing. Proper spacing makes users comfortable and creates a good experience. Too much information will confuse and distract users.
