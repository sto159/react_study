# React native란?

페이스북에서 만든 Frameworks 중 하나

Cross Platform으로 써 하나의 언어로 iOS Android 동시개발이 가능한 Opensource

#### - React의 장점

javascript를 기반으로 하기때문에 웹 node, javascript개발자들이 쉽게 입문할수 있다.

재사용률 좋다.

비용이 감소한다.

오픈소스로 풀이 넓다.

#### - React의 단점

 리엑트 만의 다른 방식(States,Props) 등을 공부해야 한다.

Native 개발방식보다는 성능이 떨어질수 있다.

오픈소스이기때문에 문제가 생기면 생산성이 떨어질수 있다.





# React 설치 & 환경변수 



패키지 매니저로 설치를 하면 여러 수고를 덜수 있기 때문에 window 기준에서 설명하겠습니다.

htttps://chocolatey.org

초코렛티 패키지 매니저로 npm node python등 한번에 설치해주기로 합니다.

사이트 접속후Get started를 눌러 아래 명령어를 복사해 관리자 권한 cmd에 복사해 설치합니다.



#### ※ 내외부 명령, 실행할수 있는 프로그램, 또는 배치파일이 아닙니다.경우

@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

를 복사 붙여넣기 해보시면 됩니다.

이후 설치 완료후 

choco -version

으로 설치 확인을 해줍니다.

이후

choco install nodejs-lts

choco install -y python2

choco install - y jdk8

npm install -g react-native-cli

를 설치하고 모두 버젼확인을 해야한다. npm도  node와 함께 깔리므로 버전확인이 필요하다.

cli은 react-native --version으로 확인하면 된다.

이후 안드로이드 스튜디오 설치.(별도로 첨부예정)

### 환경변수

window 검색창에 [ 환경 변수 ]검색

사용자 변수 - 새로만들기 - 변수이름 : ANDROID_HOME 변수값 : 

 C:\Users\user\\[사용자 이름인경우가 있음]\AppData\Local\Android\Sdk (저의 컴퓨터의 경우)

로 확인

Path - 편집 - 새로만들기 -

C:\Users\user\AppData\Local\Android\Sdk\platform-tools를 추가해 줍니다.

이후 cmd 창을 관리자 권한으로 켠 후 adb를 쳐 

android Debug...

Version 29.0 등이 뜨면 설정이 잘된것입니다.

