# CoupleConnect – Firebase Realtime Build

This build is connected to the CoupleConnect Firebase web app configuration.

## Firebase setup
1. Authentication → Sign-in method → Email/Password: Enabled.
2. Firestore Database: created.
3. Replace the Firestore Rules with the secure rules supplied with this build/instructions and Publish.

## Deploy
Upload all files to GitHub Pages (or another static HTTPS host).

## Important
The Firebase web config contains app identifiers. Security is provided by Firebase Authentication and Firestore Security Rules; never put passwords or service-account private keys in this file.
