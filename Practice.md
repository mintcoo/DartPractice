DartPractice start

## Dart

Dart의 컴파일러 기술을 사용하면 다양한 방식으로 코드를 실행할 수 있습니다.

기본 플랫폼: 모바일 및 데스크톱 장치를 대상으로 하는 앱의 경우 Dart에는 JIT(Just-In-Time) 컴파일 기능이 있는 Dart VM과 기계 코드 생성을 위한 AOT(Ahead-of-Time) 컴파일러가 모두 포함되어 있습니다.

웹 플랫폼: 웹을 대상으로 하는 앱의 경우 Dart는 개발 또는 프로덕션 목적으로 컴파일할 수 있습니다. 웹 컴파일러는 Dart를 JavaScript로 변환합니다.

https://dart.dev/overview

## How To Learn

https://dartpad.dev << 들어가서 하거나

![image-20230825215744445](Practice.assets/image-20230825215744445.png)

- VSCode 사용시 flutter extension 깔아보기

  -  vscode에서 하려고 flutter 설치하셨는데 sdk 설치하라고 안내문 

    vscode 관리자 권한으로 들어가셔서, 터미널에

    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

    ↑↑ 이거 입력 후

    choco install dart-sdk

    ↑↑ 이거 입력

    ** 설치할때 bash에서 말고 그냥 powershell터미널에서 하니까 됨

