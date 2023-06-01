<details>
  <summary>Git이란? (2)</summary>

  - 코드 버전 관리를 할 수 있는 프로그램입니다.
  - GitHub를 통해 협업을 가능하게 해줍니다.
</details>

<details>
  <summary>Git의 역사에 대해 설명해주세요. (5(10))</summary>

  - 리누스 토발즈가 리눅스를 만든 이후에 BitKeeper라고 하는 툴로 리눅스의 각 버전들을 관리하고 있었습니다.
  - BitKeeper가 유료화된 후 리누스 토발즈는 본인이 직접 버전 관리 프로그램인 Git을 만들었습니다.
  - Git은 당시에 아래와 같은 목표를 갖고 설계 및 제작되었습니다.
    - 빠른 속도
    - 단순한 디자인
    - 비선형적 개발 지원
    - 완전 분산형 시스템
    - 리눅스와 같은 거대한 프로젝트도 속도 저하의 문제없이 관리할 수 있는 시스템
  - Git은 버전 관리(version control), 협업(cooperation)에 필요한 여러 요소들이 고려되었기 때문에, 사용성이 굉장히 좋은 프로그램이 될 수 있었습니다.
  - Git의 뜻
    - "git" can mean anything, depending on your mood
    - 유닉스 커맨드에서 사용되는 명령어 이름을 제외한 랜덤한 알파벳 3글자의 조합
    - 멍청하고 단순한(이런 특성을 지닌 아무 단어로 해석되어도 좋다는 의미)
    - global information tracker의 약자
    - goddamn idiotic truckload of shit이라는 욕설의 약자
</details>

<details>
  <summary>GitHub란? (1)</summary>

  - Git으로 관리하는 프로젝트를 올려둘 수 있는 원격 저장소를 제공해주는 사이트입니다.
</details>

<details>
  <summary>Repository란? (2)</summary>

  - 프로젝트 디렉토리 내의 .git 디렉토리입니다.
  - 프로젝트의 변경 사항들(commit)이 저장되어 있습니다.
</details>

<details>
  <summary>Commit이란? (2)</summary>

  - 프로젝트 디렉토리의 모습을 하나의 버전으로 남기는 동작과 결과물입니다.
  - 커밋하는 당시의 프로젝트 디렉토리의 모습이 스냅샷처럼 레포지토리에 저장됩니다.
</details>

<details>
  <summary>Repository를 만드는 법은? (1)</summary>

  - `git init PATH` 명령어로 비어있는 레포지토리(.git 파일)을 생성합니다.
</details>

<details>
  <summary>Commit하는 방법은? (3(7))</summary>

  - 처음으로 커밋을 하기 전에 사용자의 이름과 이메일 주소를 설정해야 합니다.
    - `git config user.name "user_name"
    - `git config user.email "user_email"
  - 커밋 하기 전에 working directory 상의 변경 내용을 staging area에 추가해야 합니다.
    - `git add path1 path2 ...
    - `-A` 옵션을 사용하면 최상위 디렉토리에서 `git add .`를 한 것처럼 어디에 위치하든 항상 모든 변경 내용을 add합니다.
    - `-p` 옵션을 사용하면 모든 변경 내용을 확인하면서 add할 수 있습니다.
    - `git status`로 staging area의 상태를 볼 수 있습니다.
  - `git commit -m "commit message"
</details>

<details>
  <summary>Git의 3가지 작업 영역은? (3)</summary>

  - working directory: 작업을 하는 프로젝트 디렉토리입니다.
  - staging area: git add를 한 파일들이 존재하는 영역으로 커밋을 하게되면 staging area에 있는 파일들만 커밋에 반영됩니다.
  - repository: 커밋들이 저장되는 영역입니다.
</details>

<details>
  <summary>Git이 보는 파일의 4가지 상태는? (2(3))</summary>

  - Untracked: 한 번도 staged된 적 없는 상태
  - Tracked: staged된 적 있는 상태
    - Unmodified: 최신 커밋의 모습과 비교했을 때 수정 사항이 없는 상태
    - Modified: 최신 커밋의 모습과 비교했을 때 수정 사항이 있는 상태
    - Staged: 파일의 내용이 수정되고나서 staging area에 올라와있는 상태
</details>

<details>
  <summary>git add를 취소하는 방법은? (1)</summary>

  - `git reset path1 path2 ...` 명령어로 stging area에서 파일을 제거합니다.
</details>

<details>
  <summary>Local repository와 remote repository를 연결하는 방법은? (5(2(3)))</summary>

  - 초기 설정
    - `git remote add origin github_url`
    - `git push -u origin branch_name`
      - `-u` = `--set-upstream` tracking connection 형성
      - local repository의 branch만 입력해도 remote repository에 같은 이름의 branch로 push됩니다.
      - tracking connection이 없으면 `git push origin <LOCAL_BRANCH>:<REMOTE_BRANCH> 형태로 push해야 합니다.
  - `git push` 로컬 레포지토리의 변경 사항을 리모트 레포지토리에 반영합니다.
  - `git pull` 리모트 레포지토리의 변경 사항을 로컬 레포지토리에 반영합니다.
  - push와 pull은 작업 단위가 브랜치입니다.
  - 자신과 collaborator만 push할 수 있습니다.
</details>

<details>
  <summary>다른 프로젝트를 가져오는 방법은? (1)</summary>

  - `git clone URL` 명령어로 리모트 레포지토리를 다운로드합니다.
</details>

<details>
  <summary>Github license란? (2)</summary>

  - [Licensing a repository - GitHub Docs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository#choosing-the-right-license)
  - [Github license의 종류와 나에게 맞는 라이선스 선택하기 | by FlyingSquirrel | Medium](https://flyingsquirrel.medium.com/github-license%EC%9D%98-%EC%A2%85%EB%A5%98%EC%99%80-%EB%82%98%EC%97%90%EA%B2%8C-%EB%A7%9E%EB%8A%94-%EB%9D%BC%EC%9D%B4%EC%84%A0%EC%8A%A4-%EC%84%A0%ED%83%9D%ED%95%98%EA%B8%B0-ae29925e8ff4)
</details>

<details>
  <summary>오픈 소스 프로젝트의 역사에 대해 설명해주세요. (5(3))</summary>

  - 오픈 소스 프로젝트(open source project)란 소스 코드가 공개되어 있는 프로젝트입니다.
  - 1983년 리차드 스톨만(Richard Stallman)이라고 하는 MIT의 연구원이 자유 소프트웨어 운동을 시작했습니다.
  - 리차드 스톨만은 자유 소프트웨어 재단(Free Software Foundation)이라는 걸 세우고 이러한 운동을 조직화 했습니다.
  - 자유 소프트웨어 제단의 철학
    - 소프트웨어는 소스 코드가 공개되어야 한다.
    - 소프트웨어는 누구나 코드를 자유롭게 가져다가 사용할 수 있어야 한다.
    - 소프트웨어는 원래의 코드를 자신이 원하는 대로 수정할 수 있어야 한다.
  - 자유 소프트웨어를 의미가 명확한 오픈 소스 소프트웨어(open source software)라고도 합니다.
</details>

<details>
  <summary>오픈 소스 소프트웨어에는 어떤 것이 있나요? (7+)</summary>

  - numpy
  - Linux
  - MySQL Server
  - WordPress
  - React Native
  - Vue.js
  - Tensorflow
</details>

<details>
  <summary>오픈 소스 프로젝트의 장단점은? (4,2)</summary>

  - 장점
    - 무료로 사용할 수 있습니다.
    - 여러 개발자들이 참여하기 때문에 코드의 신뢰도가 상대적으로 높습니다.
    - 오픈 소스 프로젝트에 참여 중인 다른 개발자들에게 질문을 할 수 있습니다.
    - 어떤 프로그램을 개발할 때 특정 분야에서 사실상 표준처럼 사용되는 오픈 소스 프로그램을 많이 활용할수록 전체 개발 속도를 단축시킬 수 있습니다.
  - 단점
    - 참여자 수가 많지 않거나 참여자의 실력이 좋지 않으면 소스 코드의 신뢰성을 보장하기 어렵습니다.
    - 해당 오픈 소스를 사용해서 문제가 생겼을 때 보상을 해주거나, 책임을 질 주체가 없습니다.
</details>

<details>
  <summary>오픈 소스 라이센스란? (1)</summary>

  - [라이선스 비교표 | 오픈소스SW 라이선스 종합정보시스템 OLIS | 오픈소스SW 라이선스 종합정보시스템 OLIS](https://www.olis.or.kr/license/compareGuide.do)
</details>

<details>
  <summary>Commit history를 보는 방법은? (2(2))</summary>

  - `git log [-n]` 명령어로 커밋 히스토리를 [n개] 출력할 수 있습니다
    - `--pretty=oneline` 옵션으로 커밋 하나당 한 줄 씩 출력할 수 있습니다.
  - `git show coomit_id` 명령어로 해당 커밋을 확인할 수 있습니다.
    - commit_id의 앞부분 4자리 이상만 입력해도 됩니다.
</details>

<details>
  <summary>최신 커밋을 수정하는 방법은? (1)</summary>

  - `git commit --amend` 명령어로 최신 커밋을 수정할 수 있습니다.
</details>

<details>
  <summary>커밋 메시지 작성 가이드라인에 대해 설명해주세요. (9(9))</summary>

  - 커밋 타입(commit type)
    - `feat`: 새로운 기능 구현
    - `fix`: 버그 수정
    - `docs`: documentation 변경
    - `style`  의미에 영향을 주지 않는, 코드 스타일에 관련된 변경 사항(포맷, 공백, 빼먹은 세미콜론, 함수 이름 변경, 줄간격, 파일 이름, 의미없는 주석 삭제)
    - `refactor` 버그를 수정하지 않고 기능을 추가하지 않는 코드 변경
    - `chore` 패키지 매니저 설정, 코드 수정 없는 설정 변경 등
  - 커밋 메시지의 제목과 상세 설명 사이에는 한 줄을 비워두세요
  - 커밋 메시지의 제목 뒤에 온점(.)을 붙이지 마세요
  - 커밋 메시지의 제목의 첫 번째 알파벳은 대문자로 작성하세요
  - 커밋 메시지의 제목은 명령조로 작성하세요
  - 커밋 메시지의 제목은 영문 기준 50자 이내로 작성하세요
  - 커밋 메시지의 본문은 영문 기준 72자마다 줄을 바꿔주세요
  - 커밋의 상세 내용에는 이런 걸 적으면 좋습니다
    - 왜 커밋을 했는지
    - 어떤 문제가 있었고
    - 적용한 해결책이 어떤 효과를 가지는지
  - 다른 사람들이 자신의 코드를 바로 이해할 수 있다고 가정하지 말고 최대한 친절하게 작성하세요
</details>

<details>
  <summary>커밋 가이드라인에 대해 설명해주세요. (2)</summary>

  - 하나의 커밋에는 하나의 수정사항, 하나의 이슈를 해결한 내용만 남기도록 하세요
  - 현재 프로젝트 디렉토리의 상태가 그 내부의 전체 코드를 실행했을 때 에러가 발생하지 않는 상태인 경우에만 커밋을 하도록 하세요
</details>

<details>
  <summary>두 커밋 간의 차이를 보는 방법은? (1(4))</summary>

  - `git diff`
    - `--staged`: 커밋된 파일과 add된 파일 비교
    - `[commit_id1] [commit_id2]`: 커밋 간의 비교
    - `HEAD HEAD^`: HEAD와 그 전의 커밋 비교
    - `[branch1] [branch2]`: branch 간의 비교
</details>

<details>
  <summary>HEAD란? (3)</summary>

  - Working directory를 구성하는 브랜치(커밋)을 가리키는 포인터입니다. 
  - `HEAD^`: HEAD가 가리키는 커밋의 바로 이전 커밋입니다.
  - `HEAD~n`: HEAD가 가리키는 커밋의 n단계 전의 커밋입니다.
</details>

<details>
  <summary>이전 커밋으로 git reset하는 방법은? (1(4))</summary>

  - `git reset --option commit_id` 명령어로 HEAD가 해당 커밋을 가리키게 합니다.
    - `--hard`: working directory와 staging area 모두 변경합니다.
    - `--mixed`: working directory만 변경합니다.
    - `--soft` working directory와 staging area 모두 변경하지 않습니다.
    - `git reflog` 명령어로 커밋 히스토리에서 사라진 커밋 id를 확인하고 다시 reset하여 복구할 수 있습니다.
</details>

<details>
  <summary>커밋에 tag를 다는 방법은? (3)</summary>

  - `git tag tag_name commit_id` 명령어로 커밋에 태그를 달 수 있습니다.
  - `git tag` 명령어로 프로젝트 디렉토리 내의 모든 태그를 조회할 수 있습니다.
  - `git tag -d tag_name` 명령어로 태그를 삭제할 수 있습니다.
</details>

<details>
  <summary>브랜치란? (1)</summary>

  - 브랜치(branch): git에서 분기되는 코드 관리의 흐름입니다.
</details>

<details>
  <summary>브랜치 명령어에 대해 설명해주세요. (10)</summary>

  - `git branch`: 모든 브랜치를 조회합니다.
  - `git branch branch_name`: 현재 커밋에 브랜치를 생성합니다.
  - `git branch -d branch_name`: 브랜치를 삭제합니다.
  - `git switch branch_name`: HEAD가 가리키는 브랜치를 변경합니다. (권장)
  - `git switch -c branch_name`: 현재 커밋에 브랜치를 생성하고 HEAD가 가리키게 합니다. (권장)
  - `git switch branch_name commit_id`: 해당 커밋에 브랜치를 생성합니다.
  - `git checkout branch_name`: HEAD가 가리키는 브랜치를 변경합니다.
  - `git checkout -b branch_name`: 현재 커밋에 브랜치를 생성하고 HEAD가 가리키게 합니다.
  - `git restore file`: 워킹 디렉토리에서 수정된 파일을 복원합니다.
  - `git restore --staged file` 파일을 staging area에서 제거합니다.
</details>

<details>
  <summary>브랜치를 merge하는 방법은? (2(2))</summary>

  - `git merge branch_name`: 베이스 커밋부터 대상 브랜치까지의 커밋 히스토리를 하나로 합친 내용으로 현재 위치인 브랜치에 커밋합니다.
  - 베이스 커밋으로부터 HEAD가 가리키는 브랜치에 파일 변화가 있고, merge하려는 브랜치에도 같은 파일에 다른 변화가 있다면 conflict가 발생합니다.
    - conflict가 발생한 파일들을 수정하고 커밋을 하면 해결됩니다.
    - `git merge --abort` merge를 취소할 수도 있습니다.
</details>

<details>
  <summary>HEAD와 브랜치의 관계에 대해 설명해주세요. (3(1))</summary>

  - HEAD: 브랜치의 포인터입니다.
    - `git checkout commit_id` 명령어로 HEAD가 커밋을 직접 가리키는 detached HEAD로 만들 수 있습니다.
  - 브랜치: 커밋의 포인터입니다.
  - `git reset commit_id` 명령어로 HEAD가 가리키는 브랜치가 다른 특정 커밋을 가리키게할 수 있습니다.
</details>

<details>
  <summary>merge의 종류에 대해 설명해주세요. (2(2))</summary>

  - `Fast-forward merge`: 베이스 커밋과 현재 브랜치의 커밋이 동일할 경우 빨리감기 되는 것처럼 현재 브랜치가 대상 브랜치의 커밋을 가리키게 되고 새로운 커밋을 만들지 않는 merge입니다.
  - `3-way merge`
    - 베이스 커밋의 내용과 비교했을 때 달라진 부분이 있는 것이 우선시 됩니다.
    - 두 브랜치에서 둘 다 변화가 일어났을 때에는 conflict를 발생시켜 사용자가 스스로 선택하게 합니다.
</details>

<details>
  <summary>push 전에 remote repository에 변화가 생겨 에러가 발생할 경우 어떻게 하나요? (1)</summary>

  - `git pull` 명령어로 merge를 하고 conflict가 일어난 파일들을 수정하고, 커밋하고, push하면 됩니다.
</details>

<details>
  <summary>remote repository에 있는 브랜치의 내용을 local repository에 merge하지 않고 가져오는 방법은? (2)</summary>

  - `git fetch`
  - `git diff local_branch remote_branch` 명령어로 변경점을 비교하며 가져올 수 있습니다.
</details>

<details>
  <summary>파일의 커밋 히스토리를 작성자와 함께 출력하는 방법은? (1)</summary>

  - `git blame PATH/FILE`
</details>

<details>
  <summary>커밋을 취소하는 방법은? (1(3(2)))</summary>

  - `git revert commit_id`
    - revert 후에 push하면 리모트 레포지토리에 push한 커밋을 취소할 수 있습니다.
    - 로컬 환경에서는 reset으로 커밋을 취소해도 되지만 최신 커밋이 아니기 때문에 push할 수 없습니다.
    - `commit_id1 ... commit_idN` 형태로 argument를 주면 여러 커밋을 취소할 수 있습니다.
      - commit_id1 이후 커밋부터 commit_idN 커밋까지 취소됩니다.
      - commit_id1에 해당하는 커밋은 취소되지 않습니다.
</details>

<details>
  <summary>현재 브랜치의 베이스를 다른 브랜치로 지정하는 방법은? (2)</summary>
  
  - `git reabse commit_id`
  - `git rebase --continue` 명령어로 conflict를 해결한 후 rebase를 계속 진행할 수 있습니다.
</details>

<details>
  <summary>rebase가 merge와 다른 점은? (3)</summary>
  
  - 새로운 커밋을 만들지 않습니다.
  - 커밋의 히스토리가 단순화됩니다.
  - 두 브랜치를 합쳤다는 정보가 커밋 히스토리에 남지 않습니다.
</details>

<details>
  <summary>git stash란? (8)</summary>
  
  - `git stash`: 최근 커밋 이후로 작업했던 내용을 모두 스택에 옮기고 워킹 디렉토리를 최근 커밋의 상태로 초기화 합니다.
  - `git stash list`: 스태시 스택을 살펴봅니다.
  - `git stash apply stash@{n}`: 워킹 디렉토리에 스태시를 적용합니다.
  - `git stash drop stash@{n}`: 스태시를 삭제합니다.
  - `git stash pop stash@{n}`: 워킹 디렉토리에 스태시를 적용한 후 삭제합니다.
  - 스태시의 아이디를 argument로 주지 않으면 가장 최근의 스태시를 argument로 전달합니다.
  - 어떤 브랜치에서 하던 작업을 아직 커밋하지 않았는데 다른 브랜치로 가야하는 상황에서 사용합니다.
  - 잘못된 ㅡㅂ랜치에서 작업하고 있었을 때 사용합니다.
</details>

<details>
  <summary>git cherry-pick이란? (2)</summary>
  
  - `git cherry-pick commit_id`: 원하는 작업이 들어있는 커밋들만 가져와서 현재 브랜치에 추가합니다.
  - 다른 브랜치에 있는 커밋을 선택적으로 내 브랜치에 적용시킬 때 사용합니다.
</details>

<details>
  <summary>커밋을 합치는 방법은? (1)</summary>
  
  - 이전 커밋으로 soft/mixed reset 후에 커밋을 하면 하나의 커밋에 여러 커밋 내용을 담을 수 있습니다.
</details>

<details>
  <summary>.gitignore란? (2)</summary>
  
  - git이 무시할 파일 목록입니다.
  - 워킹 디렉토리에서 버전 관리를 할 필요가 없거나 리모트 레포지토리에 공개할 수 없는 파일이나 폴더가 있다면 .gitignore 파일에 그 파일이나 폴더 이름을 추가하면 됩니다.
</details>

<details>
  <summary>Branch merge 방법들에 대해 설명해주세요. (3)</summary>
  
  - `git merge branch_name`
    - 일반적으로 많이 사용하는 merge 방법입니다.
    - 커밋 이력을 모두 남길 때 사용합니다.
    - `-ff` 옵션(fast-forward)이 기본으로 설정되어 있습니다.
    - Github의 `Merge pull request`는 `git merge --no-ff` 옵션으로 베이스 커밋이 최신 브랜치의 커밋이어도 커밋을 남기도록 강제합니다.
  - `git merge -squash branch_name`
    - 분기했던 branch에 있던 커밋 내용들을 하나로 합쳐 새로운 커밋을 만듭니다.
    - 지저분한 커밋 히스토리들을 하나로 합쳐서 기능상 의미있는 하나의 커밋만 남길 때 사용합니다.
  - Rebase & Merge
    - 분기했던 브랜치의 커밋을 최신 베이스 커밋으로 설정하고, merge하는 방법입니다.
    - 결과적으로는 `git merge -ff`와 같은 형태가 됩니다.
    - rebase를 하면 커밋들의 베이스가 변경되어 커밋 해시도 변경될 수 있습니다. 이런 경우 `git push -f` (force push)를 해야할 경우도 있습니다.
    - merge 커밋을 남길 필요가 없는 경우 사용합니다.
    - 커밋 그래프가 하나의 라인으로 그려져 가독성에 좋습니다.
</details>
