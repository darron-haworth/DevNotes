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

Get list from command prompt: >> instruments -w help
Launch specific from list: >> instruments -w "iPhone 5 (10.2) - Simulator"
