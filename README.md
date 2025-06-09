# Git

- Git은 파일의 버전을 관리하는 툴

## Git 설치

- https://git-scm.com/

![Image](https://github.com/user-attachments/assets/9c95cef9-59d3-47b3-9657-6eff9bd4becb)
![Image](https://github.com/user-attachments/assets/cc3ac318-b267-4179-ba7a-9c92c61f8bee)
![Image](https://github.com/user-attachments/assets/0938d334-fc79-4816-8fc1-c52f3a0af40b)

- `아래는 반드시 VSCode 설치하고 나서 진행하여야 함. (목록 확인 필요)`
  ![Image](https://github.com/user-attachments/assets/d52c23dd-8fb1-490e-8c70-016724a4ae0d)
- 나머지는 기본값으로 설치 완료함.

## Git 사용자 설정

- VSCode 에서 기본 터미널을 `Git Bash`로 설정함.
- 터미널 실행 단축키 : `Ctrl + ~`
- 셋팅아이콘 선택 > Setting 메뉴 선택
  ![Image](https://github.com/user-attachments/assets/bc240d83-6d2a-4624-bf7f-05cd8ae8683d)

- 검색에 `Terminal default`입력 > `Git Bash`목록 선택
  ![Image](https://github.com/user-attachments/assets/7b06c55e-9984-4e90-aa60-45e95b2c46db)

## Git 정보 확인 및 세팅(터미널에서 진행함)

- Git 버전 확인

```bash
git --version
```

- 기본 브랜치명을 main으로 설정하기(초기 설치시 master로 되어있음)

```bash
git config --global init.defaultBranch main
```

- Enter키를 통일시킴(맥, 윈도우, 리눅스가 Enter키, 줄 변경이 달리 처리됨)

```bash
git config --global core.autocrlf true
```

- Git 수정내역, 즉 commit시 메세지 상세 남기기(VSCode로 작성하도록 세팅)

```bash
git config --global core.editor "code --wait"
```

- 사용자 설정(아이디, 이메일 : 구글 계정과 GitHub 아이디 추천)

```bash
git config --global user.name "아이디"
git config --global user.email "아이디@gmail.com"
```

# GitHub

- 회원가입(https://github.com) : 구글계정
- 예제) til_git 저장소 생성 (생략)

## GitHub 사용자 계정 보안 설정

- 초기 설정시 다음 내용을 필수로 확인한다.

  - `자격 증명 관리자` > windows 자격 증명 탭 > Git 관련 제거
    ![Image](https://github.com/user-attachments/assets/4edb379d-d9a0-4de2-8bfd-caa6431d6466)

- GitHub 자격증명 등록은 git push이 진행되면 자동으로 로그인 팝업이 출력 됨.

## Git 작업 및 GitHub 연결 작업 진행

### 1. 최초 프로젝트 관리를 Git으로 설정

```bash
git init
```

### 2. 현재 프로젝트 상태 보기

```bash
git status
```

### 3. Git으로 파일 추적하기

```bash
git add README.md
```
