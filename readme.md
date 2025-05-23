# Mylo Finance Calculator

A web-based finance calculator for Mylo, built with Firebase and TailwindCSS.

## Setup Instructions

1. Clone this repository
2. Enable GitHub Pages in your repository settings
3. Make sure to set the GitHub Pages source to the main branch

## Firebase Setup

1. Go to Firebase Console
2. Enable Realtime Database
3. Set up Security Rules for your database
4. Enable Firebase Hosting

## Local Development

1. Install Firebase CLI:
```bash
npm install -g firebase-tools
```

2. Login to Firebase:
```bash
firebase login
```

3. Initialize Firebase in your project:
```bash
firebase init
```

4. Deploy to Firebase:
```bash
firebase deploy
```

## Security Note

Make sure to set up proper security rules in your Firebase Realtime Database. Here's a basic example:

```json
{
  "rules": {
    "settings": {
      ".read": true,
      ".write": "auth != null"
    },
    "credentials": {
      ".read": "auth != null",
      ".write": "auth != null"
    }
  }
}
```