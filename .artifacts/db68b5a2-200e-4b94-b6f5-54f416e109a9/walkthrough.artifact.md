# Walkthrough - Practical 3: Implicit & Explicit Intents

I have successfully implemented Practical 3, which demonstrates the use of Implicit Intents for system actions and Explicit Intents for navigating between activities.

## Changes Made

### 1. Resource Management
- **[strings.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/res/values/strings.xml)**: Added all required string resources for UI labels and hints.
- **[activity_main.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/res/layout/activity_main.xml)**: Implemented the main dashboard with buttons for various intents.
- **[activity_login.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/res/layout/activity_login.xml)**: Created a modern login screen using `MaterialCardView`.
- **Logo Fix**: Renamed the logo file to `guni_pink_logo.png` to adhere to Android resource naming conventions (no spaces or parentheses).

### 2. Application Logic
- **[MainActivity.kt](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/java/com/example/a24012011115_mad_practical_3/MainActivity.kt)**:
    - Replaced with your provided version (using package `...115...`).
    - **Implicit Intents**: Implemented logic for Browse (URL), Call (Dialer), Call Log (with permission handling), Gallery, Camera, and Alarm.
    - **Explicit Intent**: Implemented navigation to `LoginActivity`.
- **[LoginActivity.kt](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/java/com/example/a24012011115_mad_practical_3/LoginActivity.kt)**: Set up the basic activity for the login screen.

### 3. Manifest & Build Configuration
- **[AndroidManifest.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/AndroidManifest.xml)**: Added `READ_CALL_LOG` and `SET_ALARM` permissions. Registered `LoginActivity`.
- **[libs.versions.toml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/gradle/libs.versions.toml)**: Downgraded `core-ktx` to `1.15.0` to maintain compatibility with `compileSdk 36.1`.

## Verification Results

### Build Status
- **Gradle Build**: Successful (`:app:assembleDebug`).
- **Sync**: Successful.

### Implicit Intent Logic
| Action | Intent Used | Data/Extra |
| :--- | :--- | :--- |
| **Browse** | `ACTION_VIEW` | URL from EditText |
| **Call** | `ACTION_DIAL` | `tel:` + Number from EditText |
| **Call Log** | `ACTION_VIEW` | `CallLog.Calls.CONTENT_URI` |
| **Gallery** | `ACTION_VIEW` | `MediaStore.Images.Media.EXTERNAL_CONTENT_URI` |
| **Camera** | `ACTION_IMAGE_CAPTURE` | N/A |
| **Alarm** | `ACTION_SET_ALARM` | 7:30 AM, "Wake Up" |

> [!TIP]
> The app correctly requests permission for the Call Log action if it's not already granted.

## Final Task Status
- [x] UI Layouts (Main & Login)
- [x] Intent Implementation
- [x] Permission Handling
- [x] Build Configuration fixes
