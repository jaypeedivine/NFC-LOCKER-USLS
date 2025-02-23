# NFC Locker System App

This is an Android application for an NFC-based locker system. The app allows users to access lockers using NFC tags and a product key. Each user is assigned a specific locker, and access to the locker is controlled by a unique product key. The app works by writing a predefined password to an NFC tag that unlocks the assigned locker.

## Features

- **NFC Integration**: The app uses NFC (Near Field Communication) to unlock/lock lockers by writing specific passwords to NFC tags.
- **Locker Assignment**: Users are assigned a locker based on a product key.
- **Open/Close Lockers**: Once a product key is entered, users can unlock (Open) or lock (Close) their assigned locker using the app.
- **Persistent Data**: The app saves the product key and assigned locker number, allowing users to access their locker even after restarting the app.

## How It Works

1. **Locker Assignment & Product Keys**:
    - Each locker is assigned a unique product key.
    - When the user enters their product key, the app identifies the corresponding locker.
    - Example product keys: `key1` for Locker 1, `key2` for Locker 2, `key3` for Locker 3.
    
2. **Using the App**:
    - The user enters their product key in the app.
    - If the product key is valid, the app displays the assigned locker number.
    - The user can then use the **Open** button to write the locker’s password (e.g., "hi") to the NFC tag and unlock the locker.
    - The **Close** button writes a "low" command to the NFC tag, locking the locker.

## Requirements

- **Android 5.0 (Lollipop) or higher**.
- **NFC-enabled Android device** (the app will check if NFC is supported and enabled).
- **NFC tags** (the app writes to these tags for unlocking/locking lockers).

## Setup

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/yourusername/NFCLockerApp.git
    ```

2. Open the project in **Android Studio**.

3. Build and run the app on an NFC-enabled Android device.

4. Ensure that NFC is enabled on your device. The app will prompt users to turn on NFC if it is disabled.

## App Screens

1. **Product Key Screen**:
    - The user enters a product key.
    - The app verifies the key and assigns a locker.

2. **Locker Control Screen**:
    - Displays the assigned locker number.
    - Allows the user to open or close the locker using NFC.

## Known Issues

- The app only works with NFC tags and NFC-enabled devices.
- The app currently only supports 3 predefined lockers.
- Need to hard code password

Made with ❤️ by [jp](https://github.com/jaypeedivine).
