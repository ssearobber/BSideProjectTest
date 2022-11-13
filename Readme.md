# 환경설정

- 단말기 : mac
- nodejs 설치
- npm 설치
- 전체 환경 정보 : npx react-native info

안드로이드

- [공식문서](https://reactnative.dev/docs/environment-setup#node--watchman)
  - 안드로이드 스튜디오 설치
  - 에뮬레이터 : Android 12 (S)
    - Android SDK Platform 31 , Intel x86 Atom_64 System Image
  - Android SDK Build-Tools 31.0.0

ios

- [공식문서](https://reactnative.dev/docs/environment-setup#node--watchman)
  - xcode 설치(14.1)
  - sudo gem install cocoapods 설치
  - cd ./projectTest/ios && pod install 아니면 npx pod-install
  - pod 설치시 에러가 날 경우, ios폴더 안에서 pod deintegrate -> 파일삭제 명령어
  - 시뮬레이터 : ios 14 pro

# 프로젝트 시작

- 프로젝트 생성 :
  npx react-native init BSideProjectTest --template react-native-template-typescript

- 안드로이드 : npm run android
- ios : npm run ios x -> xcode에서 실행

에러 모음 :
ios에서 실행 시, Library not loaded 에러

1.  Library not loaded: @rpath/hermes.framework/hermes  
    -> https://github.com/facebook/react-native/issues/34599

# 디버거 설정

- flipper 버전 : 0.173.0
- flipper 연결 : npm i react-native-flipper --force

ios 연결
-> https://fbflipper.com/docs/getting-started/react-native/
