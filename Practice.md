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



## 변수

변수를 만드는 2가지 방법

\```
void main() {
var name = "pizza"; // 방법 1
String name = "chicken"; // 방법 2
name = "chicken ";
}
\```
함수나 메소드 내부에 지역변수를 선언할 때는 var를 사용하고
class에서 변수나 property를 선언할 때는 타입을 지정해준다.

### Dynamic Type

![image-20230828223907131](Practice.assets/image-20230828223907131.png)

- Dynamic 타입

  여러가지 타입을 가질 수 있는 변수에 쓰는 키워드이다. (해당 변수의 타입을 알 수 없을 때 주로 사용)
  변수를 선언할 때 dynamic을 쓰거나 값을 지정하지 않으면 dynamic 타입을 가진다.

  꼭 써야할때만 써야한다

  ```dart
  void main(){
      dynamic name;
      var name2;
  }
  ```

  ![image-20230828224231274](Practice.assets/image-20230828224231274.png)

  - 조건문으로 다양하게 활용가능하다
  - int면 dart에서는 홀수, 짝수 이런것들도 메서드로 제공

### Nullable Variable

- 개발자가 null 값을 참조할 수 없도록 하는 것이다.
  String뒤에 ?를 붙여줌으로서 name이 String 또는 null이 될 수 있다고 명시해준 것입니다.
  기본적으로 모든 변수는 non-nullable(null이 될 수 없음)이다.

![image-20230828224718309](Practice.assets/image-20230828224718309.png)

- null값이든 string값이든 할때는 물음표

![image-20230828224954145](Practice.assets/image-20230828224954145.png)

![image-20230828225026251](Practice.assets/image-20230828225026251.png)

- 위에껄 단축한 문법
- 즉, nico가 null이 아니면 inNotEmpty 속성을 달라고 요청

### Final  Variables

