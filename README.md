# bnbd 홈페이지 (GitHub Pages 배포 가이드)

## 폴더 구성
- `index.html` — 홈페이지 본문
- `assets/logo.svg` — 로고 (벡터, 헤더/푸터에 사용)
- `assets/logo-512.png` — 로고 PNG (512x512)
- `assets/favicon-32.png`, `assets/favicon-180.png` — 파비콘

## GitHub Pages로 배포하는 방법
1. GitHub에서 새 저장소 생성 (예: `bnbd`)
2. 이 폴더(`bnbd_site`)의 모든 파일을 그 저장소 루트에 업로드/푸시
   ```
   git init
   git add .
   git commit -m "bnbd 홈페이지"
   git branch -M main
   git remote add origin https://github.com/<계정명>/<저장소명>.git
   git push -u origin main
   ```
3. GitHub 저장소 → **Settings → Pages**
4. Source: **Deploy from a branch**, Branch: **main / (root)** 선택 후 저장
5. 몇 분 뒤 `https://<계정명>.github.io/<저장소명>/` 에서 접속 가능
   - 저장소 이름을 `<계정명>.github.io`로 만들면 루트 도메인으로 바로 서비스됩니다.

## 수정하고 싶을 때
- 텍스트/문구: `index.html`에서 직접 수정
- 이메일/연락처: `index.html` 내 `sosim13p@gmail.com` 검색 후 교체
- 색상: `index.html` 상단 `<style>` 안 `--indigo`, `--violet` 값 변경
- 로고: `assets/logo.svg` 교체 (같은 파일명 유지하면 코드 수정 불필요)

## 구글 플레이 개발자 계정 등록용 안내
등록 시 웹사이트 URL 항목에 위에서 발급받은 GitHub Pages 주소
(`https://<계정명>.github.io/<저장소명>/`)를 입력하시면 됩니다.
