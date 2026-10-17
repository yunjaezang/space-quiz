# 궤도 너머 · 우주 탐험 퀴즈

태양계와 우주에 관한 10문제를 풀고 해설을 읽는 한국어 퀴즈 앱입니당.
정답당 10점씩 최대 100점을 얻으며, 결과 화면에서 오답을 복습할 수 있당.
모바일 화면, 라이트·다크 모드와 키보드 조작을 지원한당.

## 로컬 실행

저장소를 내려받은 뒤 `index.html`을 브라우저에서 직접 열면 된당.
Windows PowerShell에서는 저장소 폴더에서 다음 명령을 실행한당.

```powershell
Start-Process .\index.html
```

HTML, CSS, JavaScript와 SVG가 모두 `index.html`에 포함되어 있어
패키지 설치, 빌드, 로컬 서버 또는 외부 자산이 필요하지 않당.
선택지는 클릭하거나 숫자 `1`–`4`로 고르고, 답변 후 다음 버튼으로 이동한당.

## GitHub Pages 배포

사이트 주소: <https://yunjaezang.github.io/space-quiz/>

저장소의 **Settings → Pages → Build and deployment → Source**는
**GitHub Actions**로 설정한당.
`.github/workflows/pages.yml`은 PR에서 게시 파일 준비를 확인하고,
`main`에 변경 사항이 반영되면 GitHub Pages에 자동 배포한당.
Actions의 **Deploy to GitHub Pages → Run workflow**에서도 `main`을 선택해
수동으로 배포할 수 있당.

별도 컴파일 없이 `index.html`만 게시 아티팩트에 담으므로
README와 저장소 설정 파일은 사이트에 포함되지 않는당.
배포 결과는 Actions 실행 내역과 `github-pages` 환경에서 확인한당.
