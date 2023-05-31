<details>
  <summary>유닉스란? (1(3))</summary>
  <br />
  
  - 유닉스(Unix)는 1970년대 초반에 개발된 운영체제입니다.
    - 소프트웨어를 개발하고 실행할 수 있는 편리한 플랫폼
    - 쉽게 수정해서 다른 컴퓨터에 적용 가능
    - 유닉스 운영 체제: macOS, Linux, Ubuntu, ...
</details>

<details>
  <summary>유닉스의 시작과 변형에 대해 설명해주세요. (3)</summary>
  <br />
  
  - 유닉스는 1970년 초반, 미국 벨 연구소 직원 켄 톰슨과 데니스 리치의 주도로 개발자들이 소프트웨어를 개발하고 실행할 수 있는 편리한 플랫폼을 제공하기 위해 개발되었습니다.
  - C로 대부분 작성되었기 때문에 수정해서 다른 컴퓨터에 적용하기 편리했습니다.
  - 다양한 버전의 유닉스가 만들어져 변형에 제한을 두기 위해 POSIX라는 유닉스의 표준이 만들어졌습니다.
</details>

<details>
  <summary>무료와 공유의 문화, 리눅스의 등장에 대해 설명해주세요. (6)</summary>
  <br />
  
  - 유닉스를 사용하거나 변형할 때, AT&T에 라이센스 비용을 지불해야 했습니다.
  - 그래서 Free Software Foundation에서 유닉스의 코드를 하나도 사용하지 않고 유닉스와 유사한 운영 체제 GNU를 직접 만들어 무료로 배포했습니다.
  - GNU: "GNU's Not Unix!"
  - 핀란드에서 헬싱키 대학교를 다니던 리누스 토발즈라는 학생이 Linux라는 커널을 완성했습니다.
  - GNU 프로젝트에서 Linux를 가져다 쓰기로 했고, GNU/Linux가 완성되었습니다.
  - 그 후 Ubuntu, Red hat, CentOS, Debian 등 GNU/Linux를 변형한 리눅스 배포판들이 많이 만들어졌습니다.
</details>

<details>
  <summary>macOS에 대해 설명해주세요. (4)</summary>
  <br />
  
  - 1978년 미국 UC 버클리 대학의 대학원생이었던 Bill Joy와 Chuck Haley는 기존의 유닉스를 개량하여 BSD(Berkerly Software Distribution)라는 운영체제를 개발했습니다.
  - 스티브 잡스가 Apple 내에서 여러 갈등을 겪고 쫓겨난 후 세운 회사, NeXT라는 컴퓨터 회사에서 4.3BSD를 기반으로 NeXTStep이라는 운영 체제를 개발했습니다.
  - Apple이 외부에서 개발된 좋은 운영 체제를 가져오려는 중, NeXTStep을 가져오고, NeXT를 인수하였습니다.
  - NeXTStep을 Apple의 기기에 이식하기 위한 프로젝트를 시작했고, NeXTStep은 iOS, macOS, watchOS 등의 기초가 되었습니다.
</details>

<details>
  <summary>유닉스 운영 체제의 공통점을 설명해주세요. (5)</summary>
  <br />
  
  - POSIX라는 표준에 부합하여 공식적으로 인증을 받으면 Unix-certified, 공식 유닉스가 되고 인증받지 않고 기능적으로 거의 차이가 없는 정도라면 Unix-like, 유사 유닉스라고 부릅니다.
  - Unix-certified: macOS, HP-UX, AIX, ...
  - Unix-like: ubuntu, Red hat, Centos, Debian, ...
  - 커맨드로 운영 체제를 사용하는 관점에서는 이 모든 운영 체제들이 거의 동일합니다.
  - 그러므로 유닉스와 관련된 수많은 운영 체제들에서 유닉스 커맨드를 공통으로 사용할 수 있습니다.
</details>

<details>
  <summary>터미널이란? (1)</summary>
  <br />
  
  - 터미널(Terminal)은 인풋을 받고, 아웃풋을 출력해 주는 프로그램입니다.
</details>

<details>
  <summary>쉘 프롬프트란? (1)</summary>
  <br />
  
  - 쉘 프롬프트(shell prompt)는 유저 인풋을 받을 준비가 됐을 때마다 보여지는 메시지입니다.
</details>

<details>
  <summary>쉘과 쉘의 종류란? (1(2(10)))</summary>
  <br />
  
  - 쉘(shell)이란 쉘 언어 인터프리터로, bash와 zsh 등이 있습니다.
    - bash(Bourne again shell)
      - 본 셸을 대체하는 자유소프트웨어로서 GNU 프로젝트를 위해 브라이언 폭스(Brian Fox)가 작성한 유닉스 셀입니다.
      - bash command 문법은 거의 대부분이 sh와 호환됩니다.
      - ksh, csh에서 많은 아이디어를 받아서 command history, directory stack, $RANDOM POSIX 형식 명령어 치환 등을 지원합니다.
      - 입력 중에 명령어나 파일 이름을 자동 완성해 주는 기능도 지원합니다.
      - macOS는 10.15 Catalina 이전 버전에서 bash를 기본으로 사용했습니다.
    - zsh(Z shell)
      - 1990년에 프린스턴 대학교에 재학중이던 Paul Falastad가 zsh의 최초 버전을 작성하였습니다.
      - 상호작용 로그인 셸이자 셸 스크립트를 위한 강력한 명령 줄 인터프리터로 사용할 수 있는 유닉스 셸입니다.
      - bash, ksh, tcsh의 일부 기능을 포함하여 개선 사항이 갖추어진 확장형 본 셸입니다.
      - 커스텀이 비교적 자유로운 편입니다.
      - macOS는 10.15 버전 이후부터 zsh를 기본으로 사용합니다.
</details>

<details>
  <summary>커맨드의 기본 형태란? (1(2))</summary>
  <br />
  
  - `{command} -{options} {argument1} {argument2} ...`
    - option: command가 동작하는 방식을 지정합니다.
    - argument: command가 동작할 대상을 지정합니다.
</details>

<details>
  <summary>커맨드 매뉴얼을 보는 방법은? (1)</summary>
  <br />
  
  - `man {command}`로 커맨드 매뉴얼을 볼 수 있습니다.
</details>

<details>
  <summary>커맨드 단축키에 대해서 설명해주세요. (7)</summary>
  <br />
  
  - `Ctrl + A` 줄 가장 앞으로 커서 이동
  - `Ctrl + E` 줄 가장 뒤로 커서 이동
  - `Option + ←` 이전 단어로 커서 이동
  - `Option + →` 다음 단어로 커서 이동
  - `Ctrl + C` 실행하고 있는 작업 취소
  - `Tab` 자동 완성
  - `clear` 커맨드 라인의 스크롤을 현재 라인까지 내리는 명령어
</details>

<details>
  <summary>유닉스의 디렉토리 구조란? (8)</summary>
  <br />
  
  - `/` root directory
    - `bin`
    - `home`
      - `hopper`
      - `turing`
        - `~` user home directory
    - `tmp`
    - `usr`
</details>

<details>
  <summary>디렉토리 관련 커맨드란? (3(3))</summary>
  <br />
  
  - `pwd(print working directory)`
  - `cd(change directory) {path}`
    - path에 빈 값을 주면 `~`으로 이동
    - path에 `-` 값을 주면 `/`으로 이동
  - `ls(list) {path}`
    - path에 빈 값을 주면 working directory의 list 출력
</details>

<details>
  <summary>path의 두 종류에 대해서 설명해주세요. (3(1))</summary>
  <br />
  
  - `Absolute path` root(`/`)나 home directory(`~`)를 기준으로 하는 경로
  - `Relative path` `./`(working directory) 또는 `../`(parent directory)를 사용한 경로
    - `./`은 생략 가능
  - 폴더나 파일 이름에 공백이 들어있을 때는 따옴표나 역슬래시를 활용해야 합니다.
</details>

<details>
  <summary>ls의 중요한 옵션들에 대해 설명해주세요. (2(9(7))</summary>
  <br />
  
   - `-a`(all): 숨김 파일 표시
   - `-l`(long format): 자세한 정보 표시
     - `total`: 디렉토리에 사용하고 있는 블럭(MB)의 크기
     - 1 번째 column의 첫 글자는 파일의 종류를 나타낸다
       - `d`: directory
       - `-`: regular file
       - `l`: symoblic link
       - `p`: FIFO (named pipe)
       - `s`: socket
       - `b`,`c`: device file (block, charcter)
       - `D`: door
     - 1 번째 column의 나머지 글자는 permission 관련 내용
     - 2 번째 column은 이 파일과 연결된 링크의 개수
     - 3 번째 column은 파일의 소유자
     - 4 번째 column은 소유자가 속한 그룹
     - 5 번째 column은 파일의 크기(Byte)
     - 6 번째 column은 파일의 마지막 수정 날짜와 시간
     - 7 번째 column은 파일 이름
</details>

<details>
  <summary>Root 디렉토리의 하위 파일이란? (5(2))</summary>
  <br />
  
   - `/bin`(binaries): 유닉스 커맨드의 기본 커맨드들
   - `/sbin`: 관리자 전용 프로그램들
   - `/etc`: 각종 프로그램의 설정 파일, 관리자 권한 설정 파일 등
   - `/home` 또는 `/Users`: 사용자의 홈 디렉토리(~)
   - `/usr`: user에게 필요한 파일들
     - `/usr/bin`: 사용자가 필요한 커맨드들
     - `/usr/local`: 사용자가 직접 설치한 프로그램과 관련된 파일들
</details>

<details>
  <summary>디렉토리와 파일을 만드는 방법은? (3(2))</summary>
  <br />
  
   - `mkdir {path/dir2} {path/dir1} ...`
   - `touch {path/file1} {path/file2} ...`
     - touch는 파일의 마지막 접근 시간을 업데이트 하는 커맨드입니다.
     - 파일이 존재하지 않으면 생성합니다.
</details>

<details>
  <summary>vim 사용법은? (3(17))</summary>
  <br />
  
  - `vim {path/file}`
    - 파일을 만들거나 vim으로 파일을 엽니다.
  - `vim`의 4가지 사용 모드
    - 일반 모드(Normal Mode)
    - 입력 모드(Insert Mode)
    - 비주얼 모드(Visual Mode)
    - 명령 모드(Command Mode)
  - 단축키
    - `i` 입력 모드
    - `esc` 일반 모드
    - `v, V` 비주얼 모드(글자 단위, 줄 단위)
    - `:` 명령 모드
    - `yy` 일반 모드에서 한 줄 복사
    - `dd` 일반 모드에서 한 줄 잘라내기
    - `y` 비주얼 모드에서 지정된 영역 복사
    - `d` 비주얼 모드에서 지정된 영역 잘라내기
    - `p` 일반 모드에서 커서 위치에 붙여넣기
    - `w+enter` 명령 모드에서 파일 저장
    - `wq+enter` 명령 모드에서 파일 저장과 종료
    - `q!+enter` 명령 모드에서 파일 저장하지 않고 종료
</details>

<details>
  <summary>파일 내용을 살펴보는 방법은? (3(7(5)))</summary>
  <br />
  
 - `cat {path/file1} {path/file2} ...`
    - concatenate의 줄임말입니다.
    - 파일들의 내용을 출력합니다.
    - 파일이 여러 개인 경우 내용을 모두 붙여서 출력합니다.
 - `less {path/file}`
    - 파일의 내용을 페이지 단위로 다눠서 보여줍니다.
    - 단축키
      - 줄 이동: 위쪽 / 아래쪽 방향키
      - 다음 페이지: space 아니면 f
      - 이전 페이지: b
      - 마지막 페이지: G
      - 처음 페이지: g
 - `head/tail [-n count] PATH`
   - 파일의 첫/마지막 10줄을 출력합니다.
   - n 옵션은 출력되는 줄 개수를 바꿔줍니다.
</details>

<details>
  <summary>디렉토리와 파일을 옮기거나 이름을 변경하는 방법은? (1(2))</summary>
  <br />
  
  - `mv [-i] SOURCE_PATH DEST_PATH`
    - DEST_PATH가 이미 존재하는 디렉토리의 경로일 경우 SOURCE_PATH를 그 안으로 이동시키고, 그렇지 않으면 SOURCE_PATH의 이름을 DEST_PATH로 변경합니다.
    - i 옵션: 같은 이름의 파일이 있을 경우 덮어씌울지 확인하면서 이동합니다.
</details>

<details>
  <summary>디렉토리와 파일을 복사하거나 붙여넣는 방법은? (1(3))</summary>
  <br />
  
  - `cp [-ri] SOURCE_PATH DEST_PATH`
    - DEST_PATH가 이미 존재하는 디렉토리의 경로일 경우 SOURCE_PATH를 그 안으로 복사하고, 그렇지 않으면 DEST_PATH라는 이름으로 복사합니다.
    - r 옵션: 디렉토리를 복사할 때 필수 옵션
    - i 옵션: 같은 이름의 파일이 있을 경우 덮어씌울지 확인하면서 복사
</details>

<details>
  <summary>디렉토리와 파일을 삭제하는 방법은? (1(4))</summary>
  <br />
  
  - `rm [-rif] PATH1 PATH2 ...`
    - 경로에 해당하는 파일/디렉토리들을 지워준다
    - r 옵션: 디렉토리를 삭제할 때 필수 옵션
    - i 옵션: 확인하면서 삭제하기
    - f 옵션: 확인하지 않고 삭제하기
</details>

<details>
  <summary>Ubuntu에서 외부 프로그램을 설치하는 방법은? (1(4))</summary>
  <br />
  
  - apt
    - apt update를 하고 사용해야 합니다.
    - 관리자 권한이 필요하면 sudo 커맨드를 사용합니다.
    - `sudo apt install program` 설치
    - `sudo apt remove program` 삭제
</details>

<details>
  <summary>macOS에서 외부 프로그램을 설치하는 방법은? (1(4(1)))</summary>
  <br />
  
  - homebrew
    - homebrew에서 홈페이지 가이드대로 설치합니다.
    - `brew help` 설명
    - `brew install program` 설치
    - `brew uninstall program` 삭제
      - 남아있는 설정 파일들도 지울 수 있도록 Warning이 출력됩니다.
</details>
