# Holding Cabinet Two Companion App

Flutter companion application for the Holding Cabinet Two system.

The application provides setup, monitoring, and remote control of connected holding cabinets.

## Platform

- Flutter
- Dart
- iOS
- Android
- Web/PWA: TBD

## Connectivity

The application communicates with holding cabinets using:

- Bluetooth Low Energy (BLE) for cabinet provisioning
- Firebase Realtime Database for remote communication

During provisioning, the application configures the cabinet for Wi-Fi and Firebase connectivity.

## Firebase

Firebase project:

`Holding Cabinet Two`

Services:

- Firebase Authentication
- Firebase Realtime Database

Realtime Database:

`https://holding-cabinet-two-default-rtdb.firebaseio.com/`

The application manages Firebase user accounts and associates holding cabinets with the authenticated user.

See:

`Docs/FIREBASE.md`

## Cabinet Identification

Each cabinet has a numeric serial number.

Cabinets are associated with a Firebase user account during provisioning.

Serial-number entry method:

TBD

## MVP Functions

The companion application is intended to support:

- User account creation and login
- Cabinet provisioning
- Wi-Fi setup
- Cabinet association with the user account
- Cabinet status monitoring
- Start proof
- Stop proof
- Change proof temperature
- Change proof time

Additional application functions are TBD.

## Project Structure

Project structure will be documented as the application architecture is established.

## Development Setup

TBD

## Build and Deployment

TBD

## Documentation

- `Docs/FIREBASE.md` - Firebase authentication, Realtime Database structure, cabinet association, provisioning, and application/cabinet data interface
