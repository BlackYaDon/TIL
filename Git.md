# Git

> Git은 소스코드 형상(버전) 관리 도구이다.



> ## 기본 명령어
>
> 1. 저장소(`repository`) 만들기
>
>    ```bash
>    $ git init
>    ```
>
>    내가 원하는 폴더를 `git`으로 관리하는 저장소로 초기화한다.
>
>    (`master`)라는 표기를 통해 해당 폴더가 `git repository`라는 것을 확인할 수 있다.
>
>    (더 정확하게는 해당 폴더에 숨김 폴더로 `.git`이 있다.)
>
>    
>
> 2. `git add` - 커밋할 목록에 추가하기
>
>    ```bash
>    $ git add .
>    ```
>
>    `git add .` 에서 `.`은 현재 디렉토리를 뜻하는 리눅스 표기법이다.
>
>    현재 디렉토리의 변경 사항들을 모두 커밋할 목록에 담아둔다는 뜻이다.
>
>    `git add git.md` 라고 하면, 특정 파일만 담아둘 수도 있고, 
>
>    `git add myfolder/`라고 하면, 특정 폴더를 모두 담아둘 수도 있다.
>
>    
>
> 3.  커밋
>
>    ```bash
>    $ git commit -m '커밋메세지'
>    ```
>
>    커밋은 버전의 이력을 남기는 것이다. 
>
>    커밋할 목록에있는 내용들을 버전에 포함시킨다. (untracked / 목록에 없는 것은 포함 안됨)
>
> 4.  커밋 이력 확인하기
>
>    ```bash
>    $ git log
>    ```
>
>    
>
> 5. **git 상태 확인하기**
>
>    ```bash
>    $ git status
>    ```
>
>    CLI(Command Line Interface)에서는 현재 상태를 확인하기 위해서 지속적으로 확인해야 한다.
>
>    
>
> 6.  git global 설정하기
>
>    ```bash
>    $ git config --global user.email 'idoyon@naver.com'
>    $ git config --global user.name 'BlackYaDon'
>    ```
>
>    

## 원격 저장소 활용하기 (Github)

> 1. 원격 저장소 등록하기
>
>    ```bash
>    $ git remote add origin https://github.com/blackyadon/TIL.git
>    ```
>
>    원격 저장소 등록은 최초에 한번만 하면 된다.
>
>    위의 명령어를 통해 현재 원격 저장소가 있는지 확인 가능하다.
>
>    
>
> 2. 원격 저장소 올리기
>
>    ```bash
>    $ git pull origin master
>    ```
>
>    origin이라는 이름의 원격저장소에 올린다. (push)

