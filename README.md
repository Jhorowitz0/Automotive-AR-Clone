# 3mmscar


## Android Build Instructions

*Note a pre-requisite to these instructions for Android is that you have the Android build support modules installed through Unity Hub*

1. Add the project directory in Unity hub
2. Open the project in Unity Hub, note that you may have a different editor version and you'll receive a 'Editor version not installed' modal. Select "choose another editor". For these instructions I am using `2020.3.28f1`
3. Select the editor you wish to use and select Android for the platform.
4. Select open and confirm "Change version"
5. Click continue if you receieve a non-matching editor version modal.
6. Once the project is finished imported and processed, confirm that a checkbox appears in the Unity window in the lower right.
7. Select file > build settings > player settings
8. Under the player window select the Android tab. Modify the placeholder package name `com.DefaultCompany.mmscar` to a 3M namespace you desire.
9. Next we need to create a new secure Keystore for 3M specific builds
    1. Open the publishing settings in the same window.
    2. Select Keystore manager and open the window
    3. Select create new keystore or select an existing 3M may have
    4. Confirm the keystore file location and select open
    5. Type a secure password that you remember and confirm this password
    6. Fill out the Key alias and confirm the password again.
    7. *Add Key* should now be available to push
    8. You may get a prompt asking if you want to set this key as your project key, click yes.
    9. Now in the Android tab in the player settings enter the key password one more time below the key path.
10. In the top of the Player settings confirm the Company Name and Product name you wish to use for the Android build along with version.
11. You can close the Player settings.
12. Now on the build settings again, click build and select a location for the Android build.
