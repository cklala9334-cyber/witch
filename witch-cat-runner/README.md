# 소녀마법사랑 별빛 달리기

작은 마법사와 동료가 숲길을 달리는 한국어 2D 브라우저 게임입니다.

## 조작법

- `Space` / `↑` / 화면 탭: 점프
- `P`: 일시정지
- 모바일에서는 화면 탭과 점프 버튼을 사용할 수 있습니다.

## 로컬 실행

정적 파일이므로 폴더를 웹 서버로 열면 됩니다.

```bash
cd witch-cat-runner
python -m http.server 8080
```

브라우저에서 `http://localhost:8080`을 여세요. `file://`로 직접 열어도 대부분 동작하지만, 웹 서버를 사용하는 편이 이미지 로딩과 배포 환경을 정확히 확인할 수 있습니다.

## GitHub Pages 배포

저장소의 `witch-cat-runner` 폴더를 Pages 사이트 루트로 배포하도록 GitHub Actions가 구성되어 있습니다.

1. 저장소의 `Settings → Pages`에서 **Source: GitHub Actions**를 선택합니다.
2. `witch-cat-runner` 폴더의 파일을 커밋하고 `main` 브랜치에 push합니다.
3. `Actions` 탭의 Pages 배포가 끝나면 사이트 URL을 엽니다.

게임은 서버 API나 빌드 단계가 없는 정적 사이트라서 별도 의존성 설치가 필요 없습니다.

