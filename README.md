# CoupleConnect v4 — Real-Time Cloud Sync

This version adds automatic Firestore real-time synchronization.

## Firebase setup
1. Create a Firebase project.
2. Enable Authentication → Email/Password.
3. Create a Firestore database.
4. Register a Web App.
5. Replace the `YOUR_...` Firebase config values in `index.html`.
6. Deploy to GitHub Pages.
7. Each partner creates an account. One creates a couple code and the other joins it.

## Firestore security
Before production use, configure rules so users can only read/write couples where their UID is in `members`. Do not use open/test-mode Firestore rules.

## Current sync behavior
Goals, intimacy activities, favorites, tasks and calendar events are written to the shared document automatically after changes and are received through `onSnapshot` in real time.
