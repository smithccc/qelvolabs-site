# qelvolabs-site

Qelvo Labs 정적 웹사이트 (GitHub Pages → https://qelvolabs.com). 공개 저장소이므로 앱 코드·API 키·개인 정보·백업 파일은 넣지 않는다.

```
index.html                 Qelvo Labs 소개 · 앱 목록
404.html
CNAME                      qelvolabs.com
.nojekyll                  Jekyll 처리 끄기
tripletrack/index.html     Triple Track 소개
tripletrack/privacy/       개인정보처리방침 → /tripletrack/privacy
```

외부 스크립트·트래커·분석 도구를 넣지 않는다 (개인정보처리방침에 "추적 없음"이라고 명시).

## 수정 방법

- **개인정보처리방침 수정**: `tripletrack/privacy/index.html` 수정 → 시행일 갱신 → `git commit` & `git push` → 1~2분 뒤 자동 반영
- **새 앱 추가**: `/<앱이름>/index.html` 과 `/<앱이름>/privacy/index.html` 폴더 추가 → 루트 `index.html` 앱 목록에 한 줄 추가
- **App Store 출시 후**: `tripletrack/index.html` 의 "곧 출시" 배지를 주석 속 `[APP_STORE_URL]` 링크로 교체

## 로컬 미리보기

```bash
python3 -m http.server 8000   # → http://localhost:8000/tripletrack/privacy/
```
