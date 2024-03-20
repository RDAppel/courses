---
title: 'Web API with Express.js'
subtitle: 'Modern JavaScript'
---

# Web API with Express.js

Express.js is a web application framework for Node.js. It is designed for building web applications and APIs.

## Getting Setup

To get started with Express.js, you need to install it using npm.

<details open>
	<summary class="video">Show/Hide Video</summary>
	<div class="video-container">
		<iframe src="https://www.youtube.com/embed/" width="100%" height="100%" frameborder="0"
			allowfullscreen allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture">
		></iframe>
	</div>
</details>

Create a new directory for your project called `joke-api` and open it with Visual Studio Code.

In your project directory, create a new file called `app.js`.

Run the following commands to initialize your project and install Express.js:

```bash
npm init -y

npm install express
```

## Creating a Web API

Now we can start building our API. Take a look:

<details open>
	<summary class="video">Show/Hide Video</summary>
	<div class="video-container">
		<iframe src="https://www.youtube.com/embed/" width="100%" height="100%" frameborder="0"
			allowfullscreen allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture">
		></iframe>
	</div>
</details>

Here is the code from the video:

```javascript
const express = require('express')

const app = express()
const port = process.env.PORT || 3000

app.get('/', (request, response) => {
  response.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Server is running at http://localhost:${port}`)
})
```