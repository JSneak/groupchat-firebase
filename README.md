# Group Chat Messaging Workshop

**Table of Contents**

- [What is Firebase?](#what-is-firebase)
- [Adding Firebase to your website](#adding-firebase-to-your-website)
- [Setting up Realtime Database](#setting-up-realtime-database)
- [Pulling data from the Realtime Database](#pulling-data-from-the-realtime-database)
- [Updating data in the Realtime Database](#updating-data-in-the-realtime-database)
- [Dealing with Firebase Generated Unique Ids](#dealing-with-firebase-generated-unique-ids)
- [Conclusion](#conclusion)

The goal of this article is to expose you to the basics of Firebase and provide simple, working examples. If you want to go more in depth, check out Firebase's [documentation](https://firebase.google.com/docs/reference/js/firebase.database)

----

### What is Firebase?
Firebase is a platform that allows you to build websites without server side code. It has a ton of cool features but we are going to be focused on it's Realtime database.

Now lets get started.

---

### Adding Firebase to your website.

- Step 1: Go to console.firebase.google.com
- Step 2: Add a project
- Step 3: Press "Add Firebase to your web app"
- Step 4: Copy that code into your HTML page

### Setting up the Realtime Database

- Step 1: Go into your Database
- Step 2: Click the rules tab
- Step 3: Change your rules to the code snippet below. Normally you shouldn't do this due to security reasons, but for testing purposes it will be fine. Read more about it [here](https://firebase.google.com/docs/database/security/securing-data)
```javascript
{
  "rules": {
    ".read": "true",
    ".write": "true"
  }
}
```