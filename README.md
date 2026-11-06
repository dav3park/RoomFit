# RoomFit

RoomFit 모노레포.

| 폴더 | 내용 | 이전 레포 |
|---|---|---|
| `backend/` | Spring Boot (Java 21) API 서버 | dav3park/RoomFit-Backend |
| `web/` | React + Vite 웹 클라이언트 | dav3park/RoomFit-Web |
| `app/` | iOS (Swift, RoomPlan) 앱 | dav3park/RoomFit-App |

## CI/CD
- `.github/workflows/backend-ci.yml` — `backend/**` 변경 시 테스트 → GHCR 이미지 → EC2 배포
- `.github/workflows/web-deploy.yml` — `web/**` 변경 시 빌드 → EC2 배포

각 폴더의 커밋 히스토리는 이전 레포에서 그대로 옮겨졌습니다 (`git log -- backend/`).
