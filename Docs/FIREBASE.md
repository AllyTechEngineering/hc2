# Firebase

## Purpose

This document defines the Firebase services and Realtime Database data model used by the Holding Cabinet Two companion application.

The companion application and holding cabinet share the same Firebase user identity.

---

## Firebase Project

Project name:

Holding Cabinet Two

Realtime Database:

https://holding-cabinet-two-default-rtdb.firebaseio.com/

Database type:

Firebase Realtime Database



---

## Firebase Services

The MVP uses:

- Firebase Authentication
- Firebase Realtime Database

The companion application supports Firebase user account creation and authentication.

Firebase assigns each authenticated user a unique UID.

The UID is used as the root identifier for that user's data in the Realtime Database.

---

## Database Structure

Initial MVP structure:

```json
{
  "users": {
    "USER_UID": {
      "profile": {
        "email": ""
      },
      "cabinets": {
        "CABINET_SERIAL_NUMBER": {
          "state": {
            "mode": "idle",
            "currentTempC": 0,
            "setTempC": 0,
            "timedRun": false,
            "heaterOn": false
          },
          "command": {
            "type": "",
            "value": null
          }
        }
      }
    }
  }
}