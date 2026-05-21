# team-10
# 📌 프로젝트 제목: 채용공고 텍스트 분석 기반 "직무별 요구역량 트렌드" 연구

> **인공지능과 디지털사고 팀 프로젝트 (2단계: GitHub 중간 코드 제출)**
> 본 프로젝트는 바이브 코딩(Vibe Coding) 방식을 활용하여, 채용 플랫폼 및 기업 채용 페이지의 데이터를 수집·분석하고 인사관리(HRM) 관점의 트렌드 인사이트를 도출하는 프로그램입니다.

---

## 👥 1. 팀원 정보 및 역할 분담

| 이름 | 학과 | 학번 | 역할 분담 |
| :--- | :--- | :--- | :--- |
| **강동우** | 경영학과 | 202643101 | 데이터 정보 수집(크롤링), 분석 결과 시각화, 보고서 작성, 발표 |
| **변주빈** | 경영학과 | 202643197 | 생성형 AI 프롬프트 엔지니어링, 소스코드 최적화, 보고서 작성, 발표 |

---

## 🎯 2. 프로젝트 개요

### 💡 주제 선정 이유
채용공고는 기업이 필요로 하는 인재의 핵심 역량과 기술을 공식적으로 보여주는 가장 신뢰도 높은 데이터입니다. 이는 경영학의 **인사관리(HRM)** 분야와 밀접한 연관성을 가집니다. 채용 사이트의 데이터를 크롤링하여 산업 및 기업별 요구 역량을 비교하고, 이를 직무·연차·기업 정보와 결합(Join)하여 키워드 빈도와 변화 추이를 분석합니다. 최종적으로는 역량 요구도와 보상(연봉) 수준의 상관관계를 파악하여 현대 기업의 채용 및 보상 전략에 대한 실무적 시사점을 제안하고자 합니다.

### ❓ 핵심 연구 질문 (Research Questions)
* "현재 한국 채용시장에서 주요 직무(마케팅/재무/인사 등)별로 기업이 요구하는 핵심 역량 및 기술 키워드는 무엇인가?"
* "과거에 비해 최근 몇 년간 기업이 요구하는 역량 트렌드는 어떻게 변화하였는가?"

---

## 🛠️ 3. 사용 기술 및 개발 환경

* **언어**: Python 3.x
* **핵심 기술**: 
  * `데이터 크롤링 (Data Crawling)`: BeautifulSoup4, Selenium, Requests
  * `오픈 API 연동 (Open API)`: 공공데이터포털 고용노동부 워크넷 API
  * `데이터 전처리 및 조인 (Data Preprocessing & Join)`: Pandas, NumPy
* **협업 도구**: AI(제미나이, Claude, ChatGPT), GitHub

---

## 📊 4. 예상 데이터 소스 (Data Sources)

### 🔹 채용 플랫폼 (크롤링 및 스크래핑 대상)
* [사람인 채용 검색](https://www.saramin.co.kr/zf_user/search/recruit)
* [잡코리아 채용 리스트](https://www.jobkorea.co.kr/recruit/joblist)
* [원티드 채용 포지션](https://www.wanted.co.kr/wdlist)

### 🔹 주요 대기업 채용 페이지
* [삼성 커리어스](https://www.samsungcareers.com/) / [네이버 채용](https://recruit.navercorp.com/) / [카카오 영입](https://careers.kakao.com/) / [SK 채용](https://www.skcareers.com/)

### 🔹 공공데이터 오픈 API
* 고용노동부 워크넷(WorkNet) 채용정보 API

---

## 💻 5. 실행 방법 (How to Run)

> ⚠️ **주의**: 프로젝트 실행 전, 필요한 외부 라이브러리 설치가 필요합니다.

```bash
# 1. Repository 클론
git clone [https://github.com/공개된저장소주소.git](https://github.com/공개된저장소주소.git)

# 2. 프로젝트 디렉토리로 이동
cd team10

# 3. 필수 패키지 일괄 설치
pip install -r requirements.txt

# 4. 데이터 수집(크롤링) 스크립트 실행
python main_crawler.py
