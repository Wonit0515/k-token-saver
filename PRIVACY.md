# 개인정보처리방침 (Privacy Policy) — K-Token Saver

- **최종 수정일**: 2026-11-19
- **개발자 / 문의**: WonIT0515 (`john316foryou@gmail.com`)
- **적용 대상**: Chrome 확장 프로그램 **K-Token Saver** (Manifest V3)

---

## 1. 핵심 원칙: Zero-Server · Zero-Exfiltration

**K-Token Saver**는 사용자의 프롬프트, 대화 내용, 민감정보, 개인 식별 정보를 **어떠한 외부 서버로도 수집·전송·판매하지 않습니다.**

- 모든 한국어 프롬프트 분석, 배제 조건 분리, 코드블록 보존, 로컬 DLP 마스킹, 오프라인 라이선스(`KTK1`) 서명 검증은 **사용자 브라우저 내부(Client-Side)** 에서만 실행됩니다.
- 외부 분석 도구(Google Analytics 등), 원격 광고 SDK(Google AdSense 등), 트래킹 픽셀을 일절 탑재하지 않습니다.

---

## 2. 브라우저 로컬 저장소(`chrome.storage`) 사용 항목

확장 프로그램의 정상 동작을 위해 아래 설정과 통계만 사용자의 Chrome 로컬 저장소(`chrome.storage.local`)에 저장됩니다.

| 저장 항목 | 용도 | 외부 전송 여부 |
| :--- | :--- | :---: |
| 누적 절감 토큰·환산액 (`totalSavedTokens`, `totalSavedKrw`, `kTokenMonthlyFinOps`) | 팝업 대시보드 FinOps 절감 통계 표시 | ❌ 없음 |
| 로컬 상시 배제 규칙 (`kTokenCustomExclusions`) | 사용자가 직접 입력한 상시 제외 키워드 유지 | ❌ 없음 *(Pro 사용자가 다기기 동기화 옵션을 직접 켠 경우에만 Chrome 계정 `storage.sync` 활용)* |
| 제휴 배너 숨김·순환 상태 (`kTokenSponsorDismissedAt`, `kTokenSponsorRotationStep`) | 무료 버전 12시간 숨김 및 팁 순환 상태 유지 | ❌ 없음 |
| 오프라인 라이선스 토큰 및 Team DLP 설정 (`kTokenLicenseToken`, `kTokenDlpEnabled`, `kTokenDlpDomains`) | Pro/Team 기능 로컬 인증 및 전송 전 민감정보 마스킹 | ❌ 없음 |
| 최근 변환 이력 (`kTokenTransformHistory`, Pro 전용 최대 80건) | 팝업 내 최근 변환 이력 미리보기 및 사용자 로컬 CSV/JSON 내보내기 | ❌ 없음 |

---

## 3. 최소 권한 원칙 (Permissions)

- `storage`: 위 로컬 설정 및 통계 저장 용도로만 사용합니다.
- 호스트 권한(`https://chatgpt.com/*`, `https://claude.ai/*`, `https://gemini.google.com/*`): 사용자가 해당 AI 웹 페이지에서 단축키(`Alt+Shift+K`) 또는 플로팅 버튼을 클릭했을 때 입력창 텍스트를 로컬에서 변환·복구(`Alt+Shift+Z`)하기 위해서만 사용합니다.

---

## 4. 데이터 삭제 방법

사용자는 Chrome 확장 프로그램 관리(`chrome://extensions`)에서 K-Token Saver를 제거하거나 브라우저 확장 데이터를 초기화함으로써 로컬에 저장된 모든 설정과 통계를 즉시 완전히 삭제할 수 있습니다.

---

## 5. 문의처

개인정보 보호 또는 보안 관련 문의는 GitHub Issues 또는 이메일(`john316foryou@gmail.com`)로 연락해 주세요.
