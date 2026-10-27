# DevStudy Hub (Personal Learning Archive)

학습 기록, 알고리즘 노트, 자격증, CS, 외국어 학습을 관리하는 개인 공부 공간입니다.

- 사이트: https://licsrang.github.io/MyStudyArchive/
- 저장소: https://github.com/licsrang/MyStudyArchive
- 데이터 동기화: `licsrang/MyStudyArchive`의 `public/data/db.json`

## 로컬 실행 및 빌드

```bash
npm ci
npm run dev
```

배포용 빌드는 `npm run build`, 빌드 미리보기는 `npm run preview`로 실행합니다.

## GitHub Pages 배포

저장소의 **Settings → Pages → Build and deployment → Source**를 **GitHub Actions**로 설정합니다.
`main`에 푸시하면 `.github/workflows/deploy.yml`이 의존성 설치, 빌드, Pages 배포를 자동으로 실행합니다.
Actions 탭에서 수동 실행도 가능합니다.

```bash
git add .
git commit -m "Update study archive"
git push origin main
```

배포 상태: https://github.com/licsrang/MyStudyArchive/actions

Vite의 `base`는 저장소 이름의 대소문자를 포함한 `/MyStudyArchive/`로 설정되어 있습니다.
`npm run deploy`는 `gh-pages` 브랜치에 올리는 별도 수동 방식이므로, 위 자동 배포에서는 실행할 필요가 없습니다.
