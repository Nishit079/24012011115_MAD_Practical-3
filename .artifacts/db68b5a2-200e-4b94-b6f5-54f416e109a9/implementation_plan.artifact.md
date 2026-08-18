# Implementation Plan - Practical 3: Intent Examples & Login Screen

Implement the UI and functionality for Practical 3 using the provided code snippets.

## User Review Required
- **Package Name Consistency**: I will use `com.example.a24012011115_mad_practical_3` to match your project's current structure.
- **Logo Drawable**: Still waiting for `guni_pink_logo`. I will use a placeholder if we proceed without it.

## Proposed Changes

### Resources

#### [MODIFY] [strings.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/res/values/strings.xml)
I will populate this with the following inferred strings:
- `browse`, `web_url`, `https_www_google_com`, `enter_url`
- `call`, `phone_no`, `_9999999999`, `enter_phone_number`
- `call_log`, `call_log1`, `gallery`, `gallery1`, `camera`, `camera1`, `alarm`, `alarm1`
- `login`, `login1`, `email_id`, `password`, `hint_email`, `hint_password`, `forget_password`

#### [MODIFY] [activity_main.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/res/layout/activity_main.xml)
#### [NEW] [activity_login.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/res/layout/activity_login.xml)

### Code

#### [MODIFY] [MainActivity.kt](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/java/com/example/a24012011115_mad_practical_3/MainActivity.kt)
#### [NEW] [LoginActivity.kt](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/java/com/example/a24012011115_mad_practical_3/LoginActivity.kt)

### Manifest

#### [MODIFY] [AndroidManifest.xml](file:///C:/Users/Nishit Patel/AndroidStudioProjects/24012011115_MAD_Practical3/app/src/main/AndroidManifest.xml)

## Verification Plan
- Build the project and deploy to emulator.
- Verify all implicit intents (Browser, Dial, Call Log, Gallery, Camera, Alarm).
- Verify explicit intent (Navigate to Login).
