# 코르도바 앱 환경설정 절차
### 준비물 및 준비사항
> Android Studio / Gradle 7.3 / Java SE 8 / Apache ant 1.9.16 / node.js   
> C:\ 쪽에 HybirdApp 및 HybirdProject 폴더 만들기   
> 1. cmd을 키고 명령어 cd c:\ 을 치기   
> 2. mkdir HybirdApp 과 mkdir HybirdProject 명령어 치기(C 폴더에서 그냥 만들어도 상관 없습니다.)   
  
####  Gradle 7.3 / Java SE 8 / Apache ant 1.9.16 / node.js 설치 
> C:\HybirdApp에 Gradle 7.3 / Java SE 8 / Apache ant 1.9.16을 압축 풀기   
> 다운로드 주소   
> [Gradle](https://gradle.org/releases/) / [Java_SE_8](https://jdk.java.net/archive/) / [Apache_ant](https://ant.apache.org/bindownload.cgi) / [node.js](https://nodejs.org/ko/) / [Android_Studio](https://developer.android.com/studio?gclid=Cj0KCQiA1ZGcBhCoARIsAGQ0kkpMkg67ztQNHLwHAk9KTvjcjzZKBGghifUzjE0h6QCzYj2FjxQxIPAaAjyNEALw_wcB&gclsrc=aw.ds)   
#### 환경변수 설정하기
> 윈도우 + x을 누르고 시스템 선택 그리고 고급 시스템 설정 누르기
> 고급 탭에서 환경 변수 클릭하고 새로 만들기하여 이름과 디렉터리 경로 설정하기   
> JAVA_HOME   
> C:\HybirdApp\jdk1.8XX   
> (자바 이름이 달라도 상관없지만 반드시 JDK8이여야함.)   
> ANDROID_SDK_ROOT   
> C:\Users\(사용자명)\AppData\Local\Android\SDK or android-sdk   
> GRADLE_HOME   
> C:\gradle7.3_bin
#### 환경변수 Path 설정하기
> 고급 탭에서 환경 변수 클릭하고 시스템 변수 안에 path 라는 변수을 찾아 눌러주고 편집 누르기   
> 그 안에서 새로만들기 하여 아래의 표시 들어가게 하기   
> %JAVA_HOME%\bin   
> %ANDROID_SDK_ROOT%\tools   
> %ANDROID_SDK_ROOT%\platform-tools   
>	%ANDROID_SDK_ROOT%\build-tools   
>	%ANDROID_SDK_ROOT%\cmdline-tools\latest\bin   
>	%ANDROID_SDK_ROOT\emulator   
>	%GRADLE_HOME%\bin   
>	c:\HybridApp\apace-ant-1.9.16\bin   
> 확인 버튼 누르고 다시 환경변수에서 확인 누르기   
##### Cordova 및 Phonegap 다운로드 및 Npm 업데이트
> Node.js Command prompt 혹은 cmd 선택   
> npm / node -version 명령어 쳐서 버전 확인   
> npm update -g 명령어 치기   
> npm install -g phonegap 설치하기   
> npm install -g cordova 설치하기   
#### Android Studio에 SDK 추가 설치 및 에뮬레이터 설정하기
> Android Studio 실행하고 상단 메뉴에 Tool을 선택하고 SDK Manager 클릭   
> SDK Tools 및 SDK Platform을 클릭하고 해당 설치할 파일 설치하기   
> SDK platforms   
>	Android 12L	32   
>	Android 12	31   
>	Android 11	30   
>	Android R	29   
> SDK Tools   
>	Android SDK Tools   
>	Android SDK Platfor-tools   
>	Android SDK Build-tools   
> Extra   
>	Android Support Repository   
>	Android Auto Desktop head unit emulator   
>	Android auto API simulator   
>	Google Repository   
>	Google USB Driver   
>	Google Play Services   
>	Android SDK Command-line Tools   
>	Intel x86 Emulator Accelerator(HAXM installer)   
>	
