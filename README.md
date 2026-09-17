# 손끝IP

장인의 기술을 인정·권리화·사업화로 연결하는 손끝IP 소개 사이트입니다.
`sonkkeut-ip-homepage.md`의 설계안을 바탕으로 만든 Markdown + Jekyll 원페이지 웹사이트입니다.

## 내용 수정

- `index.md`: 홈페이지 문구와 각 섹션. HTML의 `markdown="1"` 블록 안에서도 Markdown으로 작성합니다.
- `_config.yml`: 사이트 제목, 설명, 주소, 문의 이메일. `email`에 실제 주소를 입력하면 문의 버튼이 표시됩니다.
- `assets/css/style.css`: 색상, 글꼴, 반응형 화면 구성.
- `_layouts/default.html`: 공통 메뉴, 검색·공유 메타 정보, 푸터.

## GitHub Pages 배포

1. 이 파일들을 `sonkkeut-ip/sonkkeut-ip.github.io` 저장소의 `main` 브랜치에 커밋하고 푸시합니다.
2. 저장소의 **Settings → Pages → Build and deployment**로 이동합니다.
3. Source에서 **Deploy from a branch**, Branch에서 **main**, 폴더에서 **/ (root)**를 선택하고 저장합니다.
4. Pages 빌드가 완료되면 https://sonkkeut-ip.github.io/ 에서 확인합니다.

이후 `index.md`를 수정하고 `main`에 푸시하면 GitHub Pages가 자동으로 갱신합니다.
Jekyll을 사용하므로 `.nojekyll` 파일은 추가하지 않습니다.

[GitHub Pages 공식 배포 안내](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 로컬 미리보기

Ruby와 Bundler가 설치된 환경에서 실행합니다.

```sh
bundle install
bundle exec jekyll serve
```

http://localhost:4000 에서 확인할 수 있습니다. `_config.yml`을 바꾸면 서버를 다시 실행합니다.

## 안내

현재 사업 아이디어와 계획을 소개하는 페이지입니다. 실제 선정 실적, 제휴, 매출을 의미하지 않습니다.
설계 원본 `sonkkeut-ip-homepage.md`와 README는 배포 결과에서 제외됩니다.
