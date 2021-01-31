# Chronos
This is a time management app I designed using Android Studio and Firebase. During my senior year in high school, I developed this app for an assignment and decided to publish a release version in a repository.

## Security
### To create a Chronos account
- A valid email address and a password are required to register an account and use Chronos
- The email address must contain an at symbol (@), as well as a common TLD
- Password must contain at least one number and one uppercase letter
- Password must be at least 8 characters long

### To sign in using an existing account
- The email and password used to create a Chronos account are sent as parameters in the Firebase Database method `mAuth.createUserWithEmailAndPassword(email, password)`
- Only authenticated accounts are able to access the Chronos main activity and their information

### Session persistence
- When you sign in to Chronos, your app session remains open, even if you close your application or turn off your device
- To close your session, you have to sign out inside Chronos or uninstall Chronos from your device

### Database information
- Only authenticated users are allowed to read and write information in their nodes inside Firebase Database

## Installation
- The minimum SDK version to install Chronos is 21 (Android 5.0)
- When you download the release apk from this repository, you may have to allow application downloads from unknown sources
- During installation, you may have to confirm to install an application not registered in Google Play Store or Google Play Protect

# Copyright disclaimer
Copyright 2021, Kevin Romero. All rights reserved.
