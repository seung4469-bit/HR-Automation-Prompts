---
name: ilgyeong-applicant-summary
description: 미래내일 일경험 사업의 '참여자 심사 상세' PDF에서 지원자 정보를 추출하여 1페이지 요약 카드를 생성합니다. 사용자가 "일경험 지원자 요약", "심사 상세 요약", "참여자 PDF 정리해줘" 등을 요청할 때 사용합니다.
---

# Ilgyeong Applicant Summary Skill

미래내일 일경험 사업 운영기관 실무자를 위한 지원자 요약 스킬입니다.

## 입력

- `참여자 심사 상세_*.pdf` — 고용노동부 일경험 시스템에서 다운로드한 표준 양식

## 처리 절차

1. PDF에서 다음 항목을 추출합니다.
   - 성명, 생년월일, 학력, 거주지역
   - 신청 직무, 희망 기업
   - 자기소개서 본문
   - 청년 요건 충족 여부 관련 정보

2. 추출된 데이터를 `prompts/government-program/ilgyeong-application-review.md` 의 Prompt 구조에 매핑합니다.

3. 1페이지 요약 카드를 Markdown으로 출력합니다.

## 출력 스키마
