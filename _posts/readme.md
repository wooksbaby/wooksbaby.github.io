# Jekyll 블로그 포스팅 가이드

## 1. 에디터 설정
- **추천 에디터**: Visual Studio Code (VS Code) 사용
- **이유**: Atom보다 VS Code에서의 사용 경험이 만족스러움

## 2. `_posts` 폴더 생성
- **위치**: 깃허브아이디.github.io 로컬 폴더
- **설명**: 모든 포스트 파일은 `_posts` 폴더 내에 위치해야 함

## 3. 포스트 파일 생성
- **형식**: `yyyy-mm-dd-title.md`
- **예시**: `2020-05-23-my-first-post.md`
- **확장자**: `.md`

## 4. 머릿말(Front-Matter) 작성
- **형식**:
    ```markdown
    ---
    title: " 타이틀 "
    excerpt: "md 파일에 마크다운 문법으로 작성하여 Github 원격 저장소에 업로드 해보자."
    categories:
      - Blog
    tags:
      - [Blog, jekyll, Github, Git]
    toc: true
    toc_sticky: true
    date: 2020-05-25
    last_modified_at: 2020-05-25
    ---
    ```
- **설명**: 포스트 제목, 소개 글, 카테고리, 태그, 목차 등 설정

## 5. Markdown 문법으로 내용 작성
- **형식**: Markdown 문법 사용
- **설명**: HTML보다 간편하고 효율적인 문법으로 포스트 본문 작성

## 6. 포스트 미리 보기
- **Visual Studio Code**:
    - **확장 기능**: Markdown Preview Enhanced 설치
    - **기능**: 작성 중인 문서의 웹 프리뷰 제공
- **로컬 서버**:
    - **명령어**: `bundle exec jekyll serve`
    - **URL**: `http://127.0.0.1:4000`

## 7. 포스트 업로드
- **명령어**: `git push`
- **설명**: 변동 사항을 GitHub Pages 서버에 업로드
- **VS Code**:
    - **UI 사용**: Git 기능으로 변경 사항 커밋 및 푸시

## 8. 다른 컴퓨터에서 작업
- **절차**:
    1. GitHub Repository 클론
    2. 포스트 작업 후 `git pull`로 최신 변경 사항 반영
- **설명**: 다른 컴퓨터에서 작업 시, 초기 클론 후 주기적인 `git pull` 필요
