제공해주신 'Busan Insight 2026: 공실의 역설' 프로젝트의 성격과 기술 스택에 맞춘 README.md 초안입니다. 프로젝트의 목적, 주요 기능, 데이터 출처를 명확히 기록했습니다.

📊 Busan Insight 2026: 공실의 역설 (Paradox of Vacancy)
"지표는 성장하는데, 시민은 떠나는 도시의 숨겨진 목소리"

본 프로젝트는 부산광역시의 인구 소멸 및 청년 이탈 문제를 해결하기 위해, 1,812건의 유튜브 댓글 데이터를 분석하여 정책의 실효성과 시민 체감도의 괴리를 시각화한 데이터 대시보드입니다.

📌 프로젝트 개요
부산시는 경기 부양을 위해 주택 공급 가속화 카드를 꺼냈지만, 데이터는 '일자리 부족'과 '아파트 난개발'에 대한 시민들의 피로감을 가리키고 있습니다. 이 프로젝트는 디지털 인문학(Digital Humanities) 관점에서 인구 유출의 진짜 원인을 분석하고 데이터 기반의 정책 대안을 제시합니다.

🚀 주요 기능
1. 실시간 여론 동향 (Home)
뉴스 티커: 시민들의 실제 목소리(YouTube 댓글)를 애니메이션으로 노출.

핵심 요약: 여론 감성 분석 수치(81.96% 부정) 및 최다 언급 키워드(아파트 난개발) 요약.

2. 데이터 대시보드 (Data Dashboard)
Sentiment Analysis: Chart.js를 활용한 여론 분포(부정/중립/긍정) 시각화.

Persona Toggle: '떠나는 사람'과 '남는 사람'의 관심사 차이를 비교 분석하는 인터랙티브 페르소나 카드.

Factor Analysis: 경제, 사회심리, 인프라, 정치/행정 분야별 관심도 차이 분석.

3. 심층 분석 리포트 (Insight Report)
공식 근거 매칭: 부산시 공식 통계 자료와 실제 시민 여론을 대조한 카드 섹션.

불신의 3단계 메커니즘: 우선순위 전도 → 박탈감 가속 → 유령도시 공포로 이어지는 이탈 심리 분석.

4. 정책 제언 (Policy Suggestion)
"짓는 행정"에서 "채우는 행정"으로의 패러다임 전환 제안.

에이지테크(AgeTech) 브랜딩 및 시정 신뢰 회복 방안 제시.

🛠 기술 스택
Frontend: HTML5, Tailwind CSS

Visualization: Chart.js

Icons: FontAwesome 6.4.0

Typography: Google Fonts (Noto Sans KR)

AI Collaboration: Google Gemini (댓글 분류 및 스토리북 구성)

📂 프로젝트 구조
index.html: 메인 대시보드 및 리포트 페이지

vid.mp4: 데이터 뒤의 감정을 담은 분석 영상 (로컬 경로)

assets/: (필요 시) 이미지 및 기타 리소스 저장

📊 데이터 소스 및 방법론
대상 데이터: 2025년 기준 부산 관련 주요 뉴스 채널(KNN, EBS, MBC 등) 유튜브 댓글 1,812건.

분석 방법: LLM(Large Language Model) 기반 감성 분석 및 MECE 원칙에 따른 키워드 분류.

분석 도구: n8n (워크플로우 자동화), Node.js (스크래핑), Gemini API (분석).

💻 실행 방법
별도의 서버 설정 없이 웹 브라우저에서 index.html 파일을 열어 바로 확인할 수 있습니다.

Bash

# 로컬에서 실행
open index.html
