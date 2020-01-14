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

## Deployment

- [Install Heroku Cli][install-heroku]

- Create a Heroku account

- Login via heroku cli

```
$ heroku login
```

- Create heroku app with heroku-cli and replace `{app_name}` with your preference or choose to omit it for a randomly generated name

```
$ heroku create {app_name}
```

- Push to heroku remote

```
$ git push heroku master
```


Create

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
[hosted-url]: https://node-complete-chats.herokuapp.com/chat.html?username=Yves&room=121
[install-heroku]: https://devcenter.heroku.com/articles/heroku-cli