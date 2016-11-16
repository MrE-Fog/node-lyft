Lyft + Node.js
=========

This is a WIP wrapper written in node for the [Lyft](https://www.lyft.com/developers) API. It's meant to be used alongside your existing application to quickly and easily facilitate calls to the API.

Installation
------------

First, you need to register your app in the [Lyft Developer Portal](https://www.lyft.com/developers), and take note of the `CLIENT_ID` and `CLIENT_SECRET` provided.

Next, copy `.env.sample` to `.env` and place in the root of your project, updating it with your information. Alternatively, add environment variables to your startup script. This project uses [.env](https://www.npmjs.com/package/dotenv) to manage these variables.

After registering your application, install this module in your Node.js project:

```sh
npm i node-lyft -S
```

### Initialization
-----
In order to use this module, you have to import it in your application first.

```es6
import CONFIG from './config';
import Lyft from 'node-lyft';
myApp.lyft = new Lyft(CONFIG);
```

#### Building

```sh
gulp build
```

#### Tests

```sh
gulp test
```

#### Build, Test, and Watch for changes:

```sh
gulp
```