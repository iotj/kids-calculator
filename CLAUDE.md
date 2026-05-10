# SW Multi-Agent Project

## 프로젝트 개요
멀티 에이전트 기반 SW 개발 시스템.
사용자는 PO 에이전트와만 대화하며, PO가 내부 팀을 자율 조율한다.

## 에이전트 구조
```
사용자
  ↕ (유일한 창구)
PO Agent          ← 오케스트레이터 (po-agent)
  ├─ PM Agent     ← 일정·리소스 (pm-agent)
  ├─ Dev Agent    ← 구현·기술 (dev-agent)
  ├─ Design Agent ← UX·화면설계 (design-agent)
  └─ QA Agent     ← 품질·테스트 (qa-agent)
```

## 중요 규칙
- 사용자는 PO와만 대화한다
- 내부 에이전트 이름/Task ID는 사용자에게 노출하지 않는다
- 모든 산출물은 `/outputs/` 디렉토리에 저장한다

## 파일 구조
```
.claude/
  agents/
    po-agent.md       ← PO (오케스트레이터)
    pm-agent.md       ← PM (추후 추가)
    dev-agent.md      ← Dev (추후 추가)
    design-agent.md   ← Design (추후 추가)
    qa-agent.md       ← QA (추후 추가)
  commands/
    start-project.md  ← 프로젝트 시작 커맨드
    status.md         ← 현황 보고 커맨드
CLAUDE.md             ← 이 파일
BACKLOG.md            ← 제품 백로그
outputs/              ← 산출물 저장소
```

## 현재 상태
- [x] PO 에이전트 설계 완료
- [ ] PM 에이전트 (예정)
- [ ] Dev 에이전트 (예정)
- [ ] Design 에이전트 (예정)
- [ ] QA 에이전트 (예정)
