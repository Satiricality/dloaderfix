## DeezLoader "Reborn" 3.1.4 - API Fix


![](https://extraimage.net/images/2018/06/27/4a70fcd12d83ff245ffaaea9d2287215.png)

This repository was created to fix the API of DeezLoader Reborn 3.1.3.

Easy to use software for downloading music!

## Features
- Download FLAC/MP3-320 files directly from Deezer (FLAC needs to be turned on in the options. Check 'turn on HIFI').
- Deezer library search.
- Use Deezer links as an alternative for searching and downloading.
- Support for full album downloads.
- Tagging system on MP3-320 and FLAC


## Supported platforms
- Linux x64 & x64
- Android 


# How to run
- Download the installer and run it.
- Run DeezLoader.

### How to update on Android

If you would like to update DeezLoader on Android, you need to delete the folder

```
rm -rf DeezLoader
```

Then follow from step 3.

### 1. Install Termux
In order to have DeezLoader on Android you must install `termux`.
- Play Store: [link](https://play.google.com/store/apps/details?id=com.termux)
- Apk Mirror: [link](https://www.apkmirror.com/apk/fredrik-fornwall/termux)

### 2. Install dependencies
Run `Termux` and enter those lines in order:
```
pkg update && pkg upgrade && pkg install git nodejs
```
If it asks you if you want to continue, enter `y`.

### 3. Download


To download the fixed version:
```
git clone  https://github.com/Satiricality/dloaderfix.git
```
Then navigate to the app folder using this command
```
cd DeezLoader/app
```

### 4. Install

Now lets install what we have downloaded
```
npm install
```
In order for DeezLoader to work we need to setup storage for termux
```
termux-setup-storage
```

### 5. Run

In order to run make sure that you are in DeezLoader-Reborn/app folder run
```
cd DeezLoader/app
```

Run the server side script
```
node app.js
```

And then go to your browser and enter to this site

[http://localhost:1730](http://localhost:1730)

**If you are a linux user and it returns an error or stucks at creating AppImage then go to `package.json` and delete this**

```
"win":{
	"icon": "res/icon.ico"
},
"mac":{
	"icon": "res/icon.icns"
},
```

# Credits
## Original Developer
-[ZzMTV](https://boerse.to/members/zzmtv.3378614/)

## Former Maintainers
-[ExtendLord](https://github.com/ExtendLord)<br/>
-[ParadoxalManiak](https://github.com/ParadoxalManiak)<br/>
-[snwflake](https://github.com/snwflake)<br/>
-[m0nster](https://t.me/m0nster_one)


# Disclaimer
- I am not responsible for the usage of this program by other people.
- I do not recommend you doing this illegally or against Deezer's terms of service.
- This project is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
