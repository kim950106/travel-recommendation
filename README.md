# 투어패스사업부 2025 워크숍 앱

투어패스사업부의 48시간 워크숍을 위한 모바일 우선 웹 애플리케이션입니다.

## 🚀 주요 기능

- **사용자 인증**: 이름 및 MBTI 기반 로그인
- **실시간 타이머**: 48시간 워크숍 카운트다운
- **MBTI 현황**: 참가자 MBTI 분포 및 팀별 분석
- **워크숍 일정**: 상세 프로그램 스케줄
- **설문조사**: 만족도 및 피드백 수집
- **관리자 기능**: 김현철 팀장 전용 관리 대시보드

## 🛠 기술 스택

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend**: Google Apps Script + Google Sheets
- **Design**: Pretendard 폰트, 모바일 우선 반응형 디자인
- **Deployment**: GitHub Pages 호환

## 📱 지원 기능

### 완료된 기능
- ✅ 사용자 로그인 및 세션 관리
- ✅ 워크숍 타이머
- ✅ MBTI 현황 대시보드
- ✅ 워크숍 일정 표시
- ✅ 설문조사 시스템
- ✅ 반응형 디자인

### 개발 예정
- 🔄 심리테스트 (여행 성향 분석)
- 🔄 링크 보관함
- 🔄 실시간 채팅
- 🔄 사진 갤러리

## 🚀 배포 방법

### GitHub Pages 배포
1. 이 저장소를 Fork 또는 Clone
2. GitHub에서 Settings > Pages로 이동
3. Source를 "Deploy from a branch" 선택
4. Branch를 "main"으로 설정
5. 배포된 URL로 접속

### 로컬 실행
```bash
# 저장소 클론
git clone https://github.com/your-username/tourpass-workshop-2025.git

# 폴더 이동
cd tourpass-workshop-2025

# 로컬 서버 실행 (Python 3)
python -m http.server 8000

# 브라우저에서 접속
# http://localhost:8000
```

## 🔧 백엔드 설정

### Google Apps Script 설정
1. [Google Apps Script](https://script.google.com) 접속
2. 새 프로젝트 생성
3. `backend/Code.gs` 파일 내용 복사
4. 웹 앱으로 배포
5. 배포된 URL을 `index.html`의 `API_URL`에 입력

### Google Sheets 구조
다음 시트들을 생성하세요:
- `Users`: 사용자 정보
- `Workshop_Sessions`: 워크숍 세션
- `MBTI_Data`: MBTI 분석 데이터
- `Survey_Responses`: 설문 응답
- `Link_Storage`: 링크 보관함

## 👥 참가자 정보

현재 등록된 참가자 (13명):
- 남도현 (이사)
- 김수인, 고다현, 심재희, 판티니안 (영업 1팀)
- 김현철, 이유진, 정어진, 장원준, 김대진, 손현우, 이주아, 장은진 (영업 2팀)

## 🎨 디자인 특징

- **모바일 우선**: 428px 최적화
- **브랜드 컬러**: 투어패스 블루 계열
- **타이포그래피**: Pretendard 폰트 패밀리
- **애니메이션**: 부드러운 마이크로 인터랙션
- **접근성**: 고대비, 시멘틱 마크업

## 🔐 환경 변수

개발/운영 환경 구분:
```javascript
const DEVELOPMENT_MODE = true; // 개발: true, 운영: false
```

## 📊 API 엔드포인트

| Action | Method | Description |
|--------|--------|-------------|
| `login` | POST | 사용자 로그인 |
| `getMBTIStats` | POST | MBTI 통계 조회 |
| `saveSurvey` | POST | 설문 응답 저장 |
| `saveLink` | POST | 링크 저장 |

## 🐛 알려진 이슈

- [ ] 오프라인 모드 미지원
- [ ] 푸시 알림 미구현
- [ ] 대용량 파일 업로드 제한

## 🤝 기여 방법

1. 이 저장소를 Fork
2. 새 브랜치 생성 (`git checkout -b feature/amazing-feature`)
3. 변경 사항 커밋 (`git commit -m 'Add some amazing feature'`)
4. 브랜치에 Push (`git push origin feature/amazing-feature`)
5. Pull Request 생성

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 있습니다. 자세한 내용은 `LICENSE` 파일을 참조하세요.

## 📞 연락처

프로젝트 관련 문의:
- 프로젝트 매니저: 김현철 (투어패스사업부 영업 2팀)
- 개발 지원: [GitHub Issues](https://github.com/your-username/tourpass-workshop-2025/issues)

## 🎯 로드맵

### 2025 Q1
- [x] 기본 기능 구현
- [x] MBTI 현황 대시보드
- [ ] 심리테스트 추가

### 2025 Q2
- [ ] 실시간 기능 추가
- [ ] 모바일 앱 버전
- [ ] 고급 분석 도구

---

**투어패스사업부 2025 워크숍에서 만나요! 🚀**
