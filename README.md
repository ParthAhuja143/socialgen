# Social Gen

A facebook/instagram-like inspired social media. This pet project is the rebranding of the old project 'Foodie'

![Heroku](https://heroku-badge.herokuapp.com/?app=socialgeneration) ![Vercel](https://vercelbadge.vercel.app/api/jgudo/socialgen)

## Table of contents

- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Run Locally](#run_local)
- [Deployment](#deployment)
- [Screenshots](#screenshots)

## Features

This web app consists of a basic features/functionalities of a socia media

- Login and Registration
- Notification
- Private Messaging
- Post CRUD functionality
- Comment feature
- Profile Customization
- Followers/Following feature
- Search Feature

## Technologies

| Front End    | Back End     |
| ------------ | ------------ |
| React 17.0.1 | Node 12.18.1 |
| TypeScript   | MongoDB      |
| Redux        | Mongoose     |
| Redux-Saga   | SocketIO     |
| React Router | Express JS   |
| TailwindCSS  | Passport JS  |
| PostCSS      | Cloudinary   |
| Axios        |              |

## Installation

Install `yarn` and `concurrently` as `devDependencies`

```
$ npm install yarn concurrently -D
```

To install both ends (frontend/server).

```
$ yarn init-project
```

Or to install them individually

```
$ cd frontend // or cd server and then run:
$ yarn install
```

## Run locally

Before running the project, make sure to have the following done:

- Download and install [MongoDB](https://www.mongodb.com/)
- Create [Firebase Project](https://console.firebase.google.com/u/0/) for storage bucket
- Create Google Service Account json key and configure ENV variable to your machine

Create `.env` or `.env` env variables and set the following:

```
MONGODB_URI="mongodb+srv://parth:parth@cluster0.d3amh5a.mongodb.net/?retryWrites=true&w=majority"
DB_NAME="socialgendb"
PORT=9000
CLIENT_URL="http://localhost:3000"
SESSION_SECRET="secret"
SESSION_NAME="user-session"
FIREBASE_PROJECT_ID="socialgen-8845f"
FIREBASE_STORAGE_BUCKET_URL="socialgen-8845f.appspot.com"
GOOGLE_APPLICATION_CREDENTIALS="./gcloud-service-api.json"
FACEBOOK_CLIENT_ID="1382040559234624"
FACEBOOK_CLIENT_SECRET="2e2ac3353665da50c1600f9a4f83da00"
GITHUB_CLIENT_ID="Iv1.629acfd1258e184d"
GITHUB_CLIENT_SECRET="3414cc70760f743e6f119ad42cff25ee077fafb4"
GOOGLE_CLIENT_SECRET="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"
GOOGLE_CLIENT_ID="543007274121-0n1v40qpe9bjlom6r0kbdsl9142dtt3s.apps.googleusercontent.com"
SENDGRID_API_KEY="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"
CLOUDINARY_NAME="dx26jwl31"
CLOUDINARY_API_KEY="658131229295366"
CLOUDINARY_API_SECRET="JL-_y7NGbyIbUfkhoKrVWF2WxEs"
```

You can get your Facebook client id/secret here [Facebook for developers](http://developers.facebook.com/) and for GitHub here [Register Github OAuth App](https://github.com/settings/applications/new) and set the necessary env vars above.

After doing the steps above, you have to run your `Mongo Server` and finally you can now run both ends simultaneously by running:

```
$ npm start
```

Or you can run them individually

```
$ npm run start-client // frontend
$ npm run start-server // backend

// Or you can change to individual directory then run
$ cd frontend // or cd server
$ npm start
```

## Deployment

You can deploy your react app in [Vercel](http://vercel.app/) or whatever your preferred deployment platform.
And for the backend, you can deploy your server in [Heroku](https://heroku.com)

## Screenshots

![Foodie screenshot](https://raw.githubusercontent.com/jgudo/foodie/master/frontend/src/images/screen1.png)
![Foodie screenshot](https://raw.githubusercontent.com/jgudo/foodie/master/frontend/src/images/screen2.png)
![Foodie screenshot](https://raw.githubusercontent.com/jgudo/foodie/master/frontend/src/images/screen3.png)
![Foodie screenshot](https://raw.githubusercontent.com/jgudo/foodie/master/frontend/src/images/screen4.png)
