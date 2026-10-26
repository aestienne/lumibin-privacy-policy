# LumiBin for Android TV: privacy policy

Last updated: 26 October 2026

LumiBin for Android TV ("the app", package `com.aestienne.lumibin`) is a player and organiser for your own video files: you choose the folders that hold them (or bring in a library built with the LumiBin app for Windows).

## What the app collects

**By default, nothing.** The app has no account, no sign-in, no advertising, no analytics, no crash reporting and no tracking of any kind, and no third party receives anything from the app unless you switch on the optional feature below.

## Optional: online information (off until you switch it on)

In Settings > Online information you can let the app look up posters, descriptions, ratings and episode lists. It is **off by default**. When you switch it on, the app asks these public services, over HTTPS, about the videos of your library:

- TMDB (themoviedb.org), OMDb (omdbapi.com), TVmaze (tvmaze.com), AniList (anilist.co) and Wikipedia (wikipedia.org).

What is sent: the **title and release year read from the names of your video files** (for example "The Matrix 1999"), and, for TMDB and OMDb, **the API key that you typed or loaded yourself**. Like any web request, the services also see the television's IP address. **No file, no file name beyond that title, no folder path, no watch history, no device identifier and no account** is sent, and the developer of the app runs no server and receives nothing. What comes back (posters, texts, ratings) is stored on the television. Each service handles requests under its own privacy policy. You can switch the feature off again at any time, or switch off each service on its own.

The keys are kept in the app's private storage. A keys file is read once and not kept: you choose it in Android's file picker, or the app looks for a file named `lumibin-keys` in the folders and drives of the television, only when you ask it to, and only reads that file. The keys are sent to TMDB and OMDb only to check that they work and to look titles up.

## Optional: network shares

If you add a network share (SMB or NFS) of your own NAS or computer, the app connects from the television directly to the server you named, usually on your home network. The server name, share and user name are kept in the app's private storage, and the password in Android's encrypted storage (or the app's private storage on a device that has none). They are sent only to that server, to sign in and read your videos, and never anywhere else; the developer receives nothing.

## What stays on your television

- **Your library**: the collections and folders you created, the titles, and the posters and information found online or imported from a `lumibin-library` archive, kept in the app's private storage on the television. The library itself is never sent anywhere.
- **Voice search** (optional): the microphone key of the search asks Android's speech recognition (on a Shield, the Google app) to listen. LumiBin does not record, keep or send the sound; only the words that come back are used, on the television, as the search text. What the recogniser does with the sound is covered by its own privacy policy.
- **Your settings and progress**: interface language and size, clock format, sort and filter choices, preferred audio and subtitle languages, and which titles you watched and where you stopped. They are kept in the app's private storage.
- **Your videos**: the app reads the video files in the folders you chose (on the television's storage or on network shares that your device has mounted) in order to play them. They are not copied or uploaded. The library file is copied once into the app's private cache to be imported.

The app does not back its data up to Google (Android backup is turned off).

## How the app reaches your files

There are three ways, and you choose which ones you use:

- **Network shares** that you add in the app (SMB, NFS): the app connects to your own NAS or computer by itself (see "Optional: network shares" above). No permission is needed.
- **The television's drives**, on Android 12 and earlier: when you want to add a folder of the television's memory, of a USB drive or of a network share that the television connected by itself, the app asks once for Android's "photos and media" permission (`READ_EXTERNAL_STORAGE`). The app then reads the videos and subtitles of the folders you add, by their paths. On Android 11 and 12, Android shows the app only media files (videos, pictures, sound, subtitles), not your other files; on Android 10 the permission covers the files of the storage. You can withdraw it at any time in Android's settings (Settings > Apps > LumiBin > Permissions). The app never asks for "All files access".
- **Android's own file and folder pickers** (the Storage Access Framework), for the folders you choose there and for the library file or keys file, if you use them. Android gives the app access to exactly those folders and files.

Whichever way, the app reads the names, sizes and dates of the files in the folders you added to build your library, and the video files you play (and a few of their blocks to recognise a renamed file); the library and keys files you chose are read once. Nothing read is sent anywhere. The app never changes your files and deletes one only when you ask: in "Compare files" (the menu of a held OK on a title that has several files), the bin button next to a file deletes that file for good, after a confirmation, and only where the folder lets the app delete (never on folders chosen in Android's picker). Nothing is deleted otherwise.

## Deleting your data

Uninstall the app, or clear its storage in Android's settings (Settings > Apps > LumiBin > Storage > Clear data). Everything the app keeps is then removed. Your video files and your Windows library are never touched.

## Children

The app contains no content of its own and does not collect data, from children or anyone else.

## Changes

If this policy changes, the new version will be published at the same address with a new date.

## Contact

Questions about this policy: info.lumibin@gmail.com
