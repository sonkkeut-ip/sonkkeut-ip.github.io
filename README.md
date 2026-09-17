# 손끝IP

장인의 기술을 인정·권리화·사업화로 연결하는 손끝IP 소개 사이트입니다.
`sonkkeut-ip-homepage.md`의 설계안을 바탕으로 만든 Markdown + Jekyll 원페이지 웹사이트입니다.

## 내용 수정

- `index.md`: 홈페이지 문구와 각 섹션. HTML의 `markdown="1"` 블록 안에서도 Markdown으로 작성합니다.
- `_config.yml`: 사이트 제목, 설명, 주소, 문의 이메일. `email`에 실제 주소를 입력하면 문의 버튼이 표시됩니다.
- `assets/css/style.css`: 색상, 글꼴, 반응형 화면 구성.
- `_layouts/default.html`: 공통 메뉴, 검색·공유 메타 정보, 푸터.
- `assets/pics/`: 홈페이지 설명 이미지. 원본 비율을 유지하며 화면 너비에 맞게 표시합니다.

이미지 박스는 부모 너비 이내, 최대 640px로 표시합니다. 현재 PNG는 흰 배경이 포함된 RGB 파일이며, CSS `mix-blend-mode: multiply`로 페이지 배경과 섞어 표시합니다. 이는 파일 자체의 투명화가 아니며 도식 색도 배경에 따라 조금 달라집니다. 투명 배경 PNG로 교체할 때는 해당 속성을 제거하면 원래 색을 그대로 표시할 수 있습니다.

### 이미지 배치

| 파일 | 홈페이지 위치 |
| --- | --- |
| `artisan-support-gaps.png` | 우리가 시작하는 이유 — 장인 지원의 단절 |
| `artisan-ip-management-cycle.png` | 손끝IP가 하는 일 — 통합 지원 과정 |
| `artisan-revenue-sharing.png` | 지속 가능한 수익 구조 — 기술 활용과 수익 배분 |
| `craft-knowledge-succession.png` | 우리가 그리는 다음 — 기술 기록·전승·사업화 |

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
