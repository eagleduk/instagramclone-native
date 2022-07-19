=============================   2022-07-18  ==============================
### 현재 강의 버전과 맞지 않아 사용 가능할 수도 변경이 될 수도 있다.

1. expo project create
   1. expo cli global install
        - npm install --global expo-cli

    1. expo project create
        - npx create-expo-app [`projectname`]

2. 필요 package 설치
    - ### expo 명령어가 powershell 에서는 실행되지 않는다. Command Prompt 로 변경해서 실행
   1. AppLoading
        - expo install expo-app-loading
        - 앱이 처음 시작되고 기본 설정 및 이미지등 을 import 하는 과정에서 다음 단계로 넘어가지 않게 하기 위한 Component 앱이 시작되기 전에 필요 리소스를 가지고 오는 등의 수행시간동안 화면을 잡아 둘 수 있다.
        - `startAsync`, `onError`, `onFinish` 등이 주로 쓰인다.
        - startAsync: return 값이 Promise 이어야 하며 Promise 가 정상적으로 종료가 되었을 때 onFinish, 에러가 발생했을 때 onError 를 수행
        - onError: startAsync 에서 Promise 가 정상종료가 되지 않았을 때(`reject`) 수행
        - onFinish: startAsync 에서 Promise 가 정상종료 되었을 때(`resolve`) 수행

    1. Font
        - expo install expo-font

    2. Asset
        - expo install expo-asset

    3. react-navigation
        - npm install @react-navigation/native
        - expo install react-native-screens react-native-safe-area-context
          - 현재 버전에서는 `react-native-gesture-handler, react-native-reanimated, @react-native-community/masked-view` 제외

    4. stack
        - npm install @react-navigation/native-stack