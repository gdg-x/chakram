# GDG[x] Event Web App
Standard Web App for GDG[X] Event. <br>
[Demo](https://devfest18-test.firebaseapp.com/)<br>
Version: 1.0.2

## Overview

GDG[X] Event Web App is the conference website template that helps you to set conference website with registration, speakers and schedule management in a few minutes.

The template is created by [GDG Jalandhar](https://meetup.com/GDG-Jalandhar/) team experience of running meetups.

## Features
| Feature | Description |
|---|---|
| **Fast and optimized** | 100/100 PWA on Lighthouse |
| **Works offline** | Can works offline |
| **Mobile first** | Mobo Friendly Web app can be installed as a native app on your phone |
| **SEO optimized** | index all content and get to the top in search results |
| **Speakers and schedule management** | keep and update all information in the JSON File |
| **Registration** | Attendees can register for the event using Firebase Realtime Database |


## Getting Started
1. [Fork repository](https://github.com/Vrijraj/gdgx-event-web-app/fork) and clone it locally
1. Setup Environment
   * Install Firebase CLI: `npm i -g firebase-tools` or `yarn global add firebase-tools`
1. Create [Firebase account](https://console.firebase.google.com) and login into [Firebase CLI](https://firebase.google.com/docs/cli/): `firebase login`
1. Update [Firebase Web Setup & Basic Info](/index.html), [Venue Map](/views/attending.html), [manifest.json](/manifest.json) and [Resources](/data)
1. Update Firebase.json file
  ```js 
  {
  "hosting": {
    "public": "public",
    "rewrites": [ {
      "source": "**",
      "destination": "/index.html"
    } ],
    "ignore": [
      "firebase.json",
      "**/.*",
      "**/node_modules/**"
    ]
  }
}
```

1. Run locally
   * `npm run serve` or `yarn serve`
1. Build and deploy
   * `npm run deploy` or `yarn deploy`
   
## Technology Stack

* AngularJS
* Bootstrap
* Firebase
* Service Worker
* Material Design Bootstrap


Project is published under the [MIT license](/LICENSE.md).  
Feel free to clone and modify repo as you want, but don't forget to add reference to authors :)
