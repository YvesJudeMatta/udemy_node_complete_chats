# Chat app

## Overview

Node application using web sockets to allow users to chat within chat rooms. Built while following a udemy course [The Complete Node.js Developer Course (3rd Edition)][udemy-course].

It hosted on Heroku at this [url][hosted-url].

## Run locally

Clone repo

```
$ git clone git@github.com:YvesJudeMatta/node_complete_chats.git
```

Install dependencies

```
$ cd node_complete_chats
$ npm install
```

Start server

```
$ npm run dev
```

You should now be able to preview the app on `localhost:3000`

## Deployment

### Heroku Prerequisites

[Install Heroku Cli][install-heroku]

Create a Heroku account

Login via Heroku cli

```
$ heroku login
```

### Create OR use existing heroku app

Create Heroku app with heroku-cli and replace `{app_name}` with your preference or choose to omit it for a randomly generated name

```
$ heroku create {app_name}
```

Use existing Heroku app with heroku-cli and replace `{app_name}` with your Heroku app name

```
$ heroku git:remote -a {app_name}
```

### Verify Heroku remote

You should see (fetch) and (push) for `heroku` along with your `origin` remote with the following command

```
$ git remote -v
```

### Push to Heroku remote

```
$ git push heroku master
```

## Tech stack

- Node
    - web framework
- Express
    - library for web server
- socket.io
    - library for web socket communication
- bad-words
    - filter out bad words in chat
- nodemon
    - watch files to hot reload server when files are changed
- Heroku
    - Deployment


[udemy-course]: https://www.udemy.com/course/the-complete-nodejs-developer-course-2/
[hosted-url]: http://node-complete-chats.herokuapp.com/
[install-heroku]: https://devcenter.heroku.com/articles/heroku-cli