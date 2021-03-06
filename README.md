# DevNotes


## Cleaning up a react-native project


- Delete the node_modules folder

```javascript
rm -rf node_modules && npm install
```

- Reset packager cache
```javascript
  rm -fr $TMPDIR/react-*
```
- Clear watchman watches
```javascript
  watchman watch-del-all
```

- reset npm
```javascript
npm start — —reset-cache
```

- Clean ios Build folder

## Android signing

- [Generating Signed APK](https://facebook.github.io/react-native/docs/signed-apk-android.html)

- [Storing key passwords in osx keychain](https://pilloxa.gitlab.io/posts/safer-passwords-in-gradle/)

## List iOS sims and launch specific one:

- Get list from command prompt: >> instruments -w help

- Launch specific from list: >> instruments -w "iPhone 5 (10.2) - Simulator"

### MOV to GIF from command line:
brew install ffmpeg
brew install gifsicle
cd to directory with mov file
run:

```
ffmpeg -i test.mov -s 414x736 -pix_fmt rgb24 -r 12 -f gif - | gifsicle --optimize=3 --delay=5 > test.gif
```

-r is frames per second -r 12 drops framerate from default 25 to 12

FROM: https://gist.github.com/dergachev/4627207 


### Build Android in release

react-native run-android --configuration release
