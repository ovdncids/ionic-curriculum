# Ionic
* [iOS 버전별 테스트 - TestFlight](https://developer.apple.com/kr/testflight)

## 설치
```sh
npm install -g @ionic/cli
ionic start
  Use the app creation wizard: N
    # Y일 경우 웹에서 프로젝트를 만든다.
  Framwork: Angular
  Project name: ionic-angular-study
  Starter template: tabs
  Create free Ionic account: N

cd ionic-angular-study
code .
ionic serve
```

## Capacitor 크로스 플랫폼(Cross-platform)
* https://capacitorjs.com/docs/getting-started

### Capacitor 설치
```sh
npm run build
# build 먼저 해야 함
```
```sh
npm install @capacitor/core
npm install @capacitor/cli --save-dev
npx cap init
  Name: ionic-angular-study
  Package ID: io.ionic.starter
  Create free Ionic account?: N
```

### iOS용으로 크로스 플랫폼
* XCode 설치

#### CocoaPods 설치
* https://velog.io/@jini0318/iOS-CocoaPod%EA%B3%BC-Pod-%EC%84%A4%EC%B9%98-%EB%B0%A9%EB%B2%95
```sh
sudo gem install cocoapods

# error: tool 'xcodebuild' requires Xcode, but active developer directory '/Library/Developer/CommandLineTools' is a command line tools instance
# 나중에 오류 발생할 경우
sudo xcode-select -s /Applications/Xcode.app/Contents/Developer
```

#### Capacitor iOS 생성
```sh
npm install @capacitor/ios
npx cap add ios
  # ios 폴더 생성됨
npx cap open ios
  # XCode 실행
  # XCode에서 ▶ 버튼 누르기
```

### Android용으로 크로스 플랫폼
* Android Studio 설치

#### Capacitor Android 생성
```sh
npm install @capacitor/android
npx cap add android
  # android 폴더 생성됨
npx cap open android
  # Android Studio 실행
  # Android Studio ▶ 버튼 누르기
```
