# Some Utils for OSX

## Tree

Install:
```
brew install tree
```
Use:
```javascript
~/dh_code/test/MyFancyLibrary >> tree
.
├── README.md
├── android
│   ├── build.gradle
│   └── src
│       └── main
│           ├── AndroidManifest.xml
│           └── java
│               └── com
│                   └── reactlibrary
│                       ├── RNMyFancyLibraryModule.java
│                       └── RNMyFancyLibraryPackage.java
├── index.js
├── ios
│   ├── RNMyFancyLibrary.h
│   ├── RNMyFancyLibrary.m
│   ├── RNMyFancyLibrary.podspec
│   └── RNMyFancyLibrary.xcodeproj
│       └── project.pbxproj
├── package.json
└── windows
    ├── RNMyFancyLibrary
    │   ├── Properties
    │   │   ├── AssemblyInfo.cs
    │   │   └── RNMyFancyLibrary.rd.xml
    │   ├── RNMyFancyLibrary.csproj
    │   ├── RNMyFancyLibraryModule.cs
    │   ├── RNMyFancyLibraryPackage.cs
    │   └── project.json
    └── RNMyFancyLibrary.sln

11 directories, 18 files
```

## FFmpeg
A complete, cross-platform solution to record, convert and stream audio and video
https://ffmpeg.org/
```
brew install ffmpeg
```

Converting video and audo has never been so easy.
```
ffmpeg -i input.mp4 output.avi
```
