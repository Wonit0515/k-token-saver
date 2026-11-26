# ⚡ K-Token Saver

> **100% 로컬 브라우저 구동(`<1ms`) 한국어 AI 프롬프트 최적화 · 토큰 절감 크롬 확장 프로그램**  
> Supports **ChatGPT (`chatgpt.com`)**, **Claude (`claude.ai`)**, and **Gemini (`gemini.google.com`)**

[![Chrome Web Store](https://img.shields.io/badge/Chrome%20Web%20Store-Free%20Install-2563eb?style=flat-square&logo=googlechrome&logoColor=white)](https://chromewebstore.google.com/detail/mdckdfnpajfofkfpaindnfpjjeepganh)
[![Platform](https://img.shields.io/badge/Platform-Chrome%20MV3-4f46e5?style=flat-square)](https://chromewebstore.google.com/detail/mdckdfnpajfofkfpaindnfpjjeepganh)
[![Privacy](https://img.shields.io/badge/Server%20Transmission-0%20Bytes%20(100%25%20Local)-10b981?style=flat-square)](./PRIVACY.md)
[![Sponsors](https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ea4aaa?style=flat-square&logo=githubsponsors)](https://github.com/sponsors/Wonit0515)
[![Ko-fi](https://img.shields.io/badge/Support-Ko--fi-ff5e5b?style=flat-square&logo=ko-fi&logoColor=white)](https://ko-fi.com/wonit0515)

👉 **[Chrome 웹 스토어에서 무료 설치하기 (Install on Chrome Web Store) ↗](https://chromewebstore.google.com/detail/mdckdfnpajfofkfpaindnfpjjeepganh)**

---

## ✨ 핵심 특징 (Key Highlights)

- **🔒 Zero-Server · Zero-Exfiltration (외부 서버 전송 0건)**  
  모든 한국어 구문 분석·배제 조건 분리·코드블록 보호가 **사용자 브라우저 메모리 내부(`<1ms`)**에서만 동작합니다. 입력한 프롬프트나 사내 문서가 외부 백엔드 서버로 전송되지 않습니다.
- **🗜️ Free (영구 무료 · 무제한 `초압축`)**
  - 불필요한 구어체·보조사·사족을 정리하고 핵심 과업과 배제 조건(`STRICT_EXCLUSION`)을 정돈합니다.
  - ```` ```코드블록``` ```` 및 에러 로그 원형 100% 보존 (Tier 3 가드레일).
  - 단축키 **`Alt+Shift+K`** 즉시 변환 / **`Alt+Shift+Z`** 원문 100% 복구.
  - 팝업 내 **오프라인 독립 변환기** 및 **내 로컬 상시 배제 규칙** 지원.
- **👑 Pro / Team (합리적 월 구독 예정 · 오프라인 WebCrypto 키 인증)**
  - **팀장지휘 28종 동적 라우팅** + **코드집중** + **수식계산** + 질문유형별 심층 검증선(`PRO_VERIFY`).
  - 직무 특화 스키마 팩 5종(CISO · FinOps · B2B Deal Desk · ITSM · Legal/DPA).
  - 월간 FinOps 절감 CSV/JSON 리포트 및 Team 전용 **전송 전 100% 로컬 DLP 마스킹**(API 키·JWT·PII·사내 도메인).

---

## 🚀 빠른 사용법

1. [Chrome 웹 스토어](https://chromewebstore.google.com/detail/mdckdfnpajfofkfpaindnfpjjeepganh)에서 **K-Token Saver**를 무료로 설치합니다.
2. ChatGPT, Claude, Gemini 입력창에 평소처럼 한국어로 질문합니다.
3. **`Alt+Shift+K`** (또는 우측 하단 플로팅 버튼)를 누르면 `<1ms` 내 최적화된 프롬프트로 변환됩니다.
4. 원문으로 되돌리고 싶을 때는 언제든 **`Alt+Shift+Z`** (`↩ 원문 복구`)를 누르세요.

---

## 🛡️ 개인정보 및 보안 원칙

- 본 확장 프로그램은 최소 권한(`permissions: ["storage"]`)만 요청합니다.
- 외부 광고 SDK(Google AdSense 등), 트래킹 픽셀, 원격 스크립트 로딩을 일절 사용하지 않습니다.
- 자세한 내용은 [개인정보처리방침 (PRIVACY.md)](./PRIVACY.md)을 참고해 주세요.

---

## 💬 버그 제보 · 기능 제안 · 커뮤니티 사전 참여

- 🐛 [버그 제보하기 (Bug Report)](https://github.com/Wonit0515/k-token-saver/issues/new?template=bug_report.md)
- 💡 [기능 제안하기 (Feature Request)](https://github.com/Wonit0515/k-token-saver/issues/new?template=feature_request.md)
- 📚 [신조어·오타 교정 사전 제안](https://github.com/Wonit0515/k-token-saver/issues/new?template=vocab_suggestion.yml) · [📄 `dictionary/vocab_pack.json` (CC0-1.0)](./dictionary/vocab_pack.json)
- 🧪 [익명 문장 패턴 제보 (Zero-PII)](https://github.com/Wonit0515/k-token-saver/issues/new?template=sentence_pattern.yml) · [📄 `dictionary/pattern_queue.json` (CC0-1.0)](./dictionary/pattern_queue.json)

---

## ☕ 개발 후원 (Support This Project)

K-Token Saver의 핵심 `초압축` 기능과 로컬 프라이버시 도구는 영구 무료로 제공됩니다.  
도구가 실무와 토큰 절약에 도움이 되셨다면 아래 채널로 개발을 응원해 주세요!

- 💖 **GitHub Sponsors**: https://github.com/sponsors/Wonit0515
- ☕ **Ko-fi**: https://ko-fi.com/wonit0515

---

> **Notice**: 본 저장소는 **K-Token Saver**의 공식 소개·문서·개인정보처리방침·이슈 트래커·커뮤니티 정적 사전 데이터(`CC0-1.0`) 및 후원 안내용 공개 저장소입니다. 코어 엔진 및 회귀 검증 자산은 비공개로 관리됩니다.

---

<details>
<summary>🌐 <b>English Summary</b> (Click to expand)</summary>

- **Install**: **[Install Free from Chrome Web Store ↗](https://chromewebstore.google.com/detail/mdckdfnpajfofkfpaindnfpjjeepganh)**
- **Overview**: **K-Token Saver** is a Chrome MV3 extension that refines, structures, and compresses Korean prompts **100% locally inside the browser (`<1ms`)** on ChatGPT (`chatgpt.com`), Claude (`claude.ai`), and Gemini (`gemini.google.com`) to prevent wasted LLM output tokens.
- **Free (Forever Free · Unlimited `COMPACT`)**: Cleans colloquial filler, isolates exclusions (`STRICT_EXCLUSION`), preserves code blocks/error logs, and supports offline Korean sentence polishing, `Alt+Shift+K` (optimize), and `Alt+Shift+Z` (restore original).
- **Pro / Team (Offline WebCrypto License)**: Unlocks 28 dynamic directive templates, `PRO_VERIFY` checks, 5 domain schema packs, FinOps CSV/JSON exports, and local pre-send DLP masking (API keys, JWTs, PII, custom corporate domains).
- **Privacy & Minimal Permissions**: Requests only `storage` permission and the 3 supported AI host domains; **0 bytes sent to developer servers**, no external analytics, and no remote ad SDKs or remote scripts. See [PRIVACY.md](./PRIVACY.md).
- **Community & Support**: Suggest vocabulary/patterns via GitHub Issues (`CC0-1.0` dictionaries in [`dictionary/`](./dictionary/)) or support development via [GitHub Sponsors](https://github.com/sponsors/Wonit0515) / [Ko-fi](https://ko-fi.com/wonit0515). This public repo hosts documentation, privacy policy, issue templates, and static community data only.

</details>


