# 🛡️ K-Token Saver 기업·조직 보안 아키텍처 안내 (Enterprise & Team Security)

K-Token Saver는 **사내 보안 규정상 외부 프롬프트 최적화 서버를 사용할 수 없는 조직**을 위해 설계된 Zero-Server 크롬 확장 프로그램입니다.

---

## 1. Zero-Exfiltration · 최소 권한 설계

| 보안 검증 항목 | K-Token Saver 동작 보장 |
| :--- | :--- |
| **네트워크 전송** | 기본 동작에서 **외부 개발자 서버 전송 `0 Bytes`** (모든 구문 분석·압축·다듬기 `<1ms` 브라우저 메모리 단독 실행) |
| **요청 권한** | 오직 **`permissions: ["storage"]`** 1개 + 3대 AI 채팅 호스트(`chatgpt.com`, `claude.ai`, `gemini.google.com`)만 요청 |
| **원격 코드 · 광고 SDK** | 원격 `<script>` 로딩, `eval`, Google AdSense, 외부 분석 트래킹 픽셀 **완전 배제** (`MV3 CSP` 준수) |
| **선택형 AI 연결** | `[AI 정밀 다듬기(BYOK/Ollama)]`는 기본값이 **`OFF`** 이며, 사용자가 명시적으로 켜고 사내 프록시 또는 로컬 Ollama(`127.0.0.1`)를 지정할 때만 동작 |

---

## 2. Team / Enterprise 전용 로컬 보안 기능

1. **전송 전 로컬 민감정보 마스킹 (Client-Side DLP)**
   - AWS 키, OpenAI/GitHub/Slack API 키, JWT, 이메일, 휴대폰/주민번호, 사내 비공개 IP 및 관리자가 등록한 **사내 차단 도메인**을 브라우저 내부에서 먼저 `[REDACTED_*]`로 가린 뒤 변환합니다.
   - 변환 전 원문은 로컬 메모리 Undo(`Alt+Shift+Z`)로만 유지되며 외부에 기록하지 않습니다.
2. **직무 특화 스키마 팩 5종 (CISO · FinOps · B2B Deal Desk · ITSM · Legal/DPA)**
   - 보안 거버넌스, 비용 검토, 계약/개인정보 검토 등 실무 도메인별 검증 기준을 오프라인에서 자동 결합합니다.
3. **완전 오프라인 라이선스 검증 (WebCrypto ECDSA P-256)**
   - 라이선스 인증 시에도 외부 인증 서버 호출 없이 브라우저 내 WebCrypto 공개키 서명 검증만으로 동작하므로, **폐쇄망/Strict 프록시 환경**에서도 팀 라이선스를 적용할 수 있습니다.
4. **로컬 FinOps 절감 통계 · CSV/JSON 리포트**
   - 수식 주입 방어(Formula-safe CSV escaping)가 적용된 UTF-8 BOM CSV 및 JSON 리포트를 내 PC로 직접 내려받을 수 있습니다.

---

## 3. 팀 파일럿 도입 & B2B 문의

- **공식 스토어 설치**: https://chromewebstore.google.com/detail/mdckdfnpajfofkfpaindnfpjjeepganh (`Chrome · Edge · Whale · Brave` 지원)
- **개인정보처리방침**: [PRIVACY.md](./PRIVACY.md)
- **팀/조직 도입 및 PoC 문의**: GitHub Issues 또는 `wonit0515@gmail.com` (팀 규모·원하시는 도메인 팩 요건을 함께 알려주세요)
