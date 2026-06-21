# log

## [2026-06-18] ingest — 마스터님 프로필·팀 프로필·의사결정

- 생성: [[master-profile]] (source) — 마스터님 6in1 프로필
- 생성: [[haena]] (entity) — 해나 프로필
- 생성: [[mimo]] (entity) — 미모 프로필
- 생성: [[ag]] (entity) — AG 프로필
- 생성: [[agent-team]] (concept) — 5인 에이전트 팀 체계

## [2026-06-18] decision — 지식그물 이름 '모아 (MoA)'로 확정
- knot 저장소의 공식 이름을 '모아 (MoA)'로 결정
- '지식을 모은다' + '알(Knowledge)' — 마스터님이 직접 선택
- 미모 제안 KnowNet 대신 해나 제안 '모아' 채택
- 심볼릭 링크 생성: `~/초보프로젝트/모아` → `~/초보프로젝트/knot`

## [2026-06-19] decision — 모델 전략 최종 확정 (DeepSeek + GLM-4.6V 하이브리드)

- auxiliary vision: MiMo V2.5 → **GLM-4.6V-Flash(z.ai, 무료)** 교체 완료
- 일상 대화: DeepSeek V4 Flash 유지 (GLM-4.7-Flash는 Rate Limit+품질↓로 기각)
- 생성: [[model-strategy]] (concept) — 모델 아키텍처 상세
- z.ai(글로벌) Google 로그인 가입 완료, API 키 발급
- bigmodel.cn(중국) 2,000만 토큰+2억 초대 보너스 검토 보류

- 갱신: [[master-profile]] (source) — 상세 이력, 강의 장소, 홈페이지, 거주지 추가
- 생성: [[meta-ai-labs]] (entity) — 메타 AI 랩스 협동조합 (이사진, 10대 사업, 정관)
- 생성: [[julia]] (entity) — 김소영 프로필 (학력, 자격, 경력, 저서, 예술 활동)
- 갱신: index.md — 새 페이지 2개 추가

## [2026-06-18] ingest — Hermes Studio 정보 (해나)
- 생성: [[hermes-studio]] (entity) — Hermes Studio Web UI: URL, 실행법, 접속방법, 용도 정리
- 갱신: index.md — hermes-studio 추가

## [2026-06-19] ingest — 마스터님 전체 프로젝트 로드맵 (해나)
- 생성: [[master-projects]] (concept) — 마스터님 6개 프로젝트 우선순위·데드라인 정리
- 갱신: index.md — master-projects 추가

## [2026-06-20] improvement — 3D 지식 그래프 개선 (미모)
- `knot/graph.html` 파일 개선 완료
- 변경 사항: 우주/네온 테마 배경, 자동 회전, 노드 상세 정보 팝업, 검색 기능
- 마스터님 요청에 따라 해나, AG에게 전달 완료

## [2026-06-20] addition — 카파시 가이드라인 포함 (미모)
- `knot/CLAUDE.md`에 카파시 가이드라인 추가 완료
- 핵심 원칙 6가지: 역할/맥락 명확화, 구체적 지시, 예시 제공, 단계별 설명, 출력 형식 정의, 제약조건 설정
- mimo_proxy.py 시스템 프롬프트를 통해 자동 적용

## [2026-06-21] addition — Kling AI API 정보 등록
- 생성: [[kling-api]] (entity) — Kling API 키·크레딧·사용법 정리 (3,069P)
- 갱신: index.md — kling-api 추가

## [2026-06-21] analysis — AI 영상 제작 파이프라인 (MCP 기반)
- 생성: [[ai-video-pipeline]] (concept) — N잡학교 Higgsfield MCP 사례 분석
- 5단계 파이프라인: 시나리오→마스터시트→캐릭터디자인→스토리보드→영상생성
- 캐릭터 일관성 핵심: 다각도 디자인 시트(Turnaround Sheet) 기법
- 갱신: index.md — ai-video-pipeline 추가

## [2026-06-20] skill-creation — 제드용 스킬 3개 생성 (미모)
- `~/.agents/skills/feature-dev/SKILL.md` — 개발 구조화 스킬 (7단계 워크플로우)
- `~/.agents/skills/code-review/SKILL.md` — 코드 검증 스킬 (6개 검토 항목)
- `~/.agents/skills/commit-commands/SKILL.md` — Git 커밋 자동화 스킬
- Claude Code 공식 플러그인을 참고하여 MiMo Code에 맞게 재구성
