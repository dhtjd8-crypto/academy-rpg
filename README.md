# 밝은미래 학원 RPG — PWA 배포 가이드

## 📁 파일 구성
```
academy-rpg/
├── index.html      ← 앱 전체 (로그인, 캐릭터 생성, 학생/강사/원장 화면)
├── manifest.json   ← PWA 설정 (앱 이름, 아이콘, 색상)
├── sw.js           ← 서비스 워커 (오프라인 지원)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

---

## 🚀 Netlify로 5분 배포 (무료, 가장 쉬움)

1. https://netlify.com 접속 → 회원가입 (무료)
2. "Deploy manually" 클릭
3. **academy-rpg 폴더 전체**를 드래그앤드롭
4. 배포 완료! 링크가 생성됨 (예: `https://academy-rpg-12345.netlify.app`)

---

## 📱 카톡으로 공유하는 법

1. 위 Netlify 링크를 카톡으로 친구에게 전송
2. 친구가 링크 클릭 → 브라우저로 열림
3. 브라우저 상단 "홈화면에 추가" 선택
4. 앱 아이콘이 생성되고 앱처럼 실행됨!

---

## 📲 홈화면 추가 방법

### 아이폰 (Safari)
1. Safari에서 앱 URL 열기
2. 하단 공유 버튼(□↑) 탭
3. "홈 화면에 추가" 선택
4. "추가" 탭

### 안드로이드 (Chrome)
1. Chrome에서 앱 URL 열기
2. 상단에 "앱 설치" 배너가 자동으로 뜸
3. "설치" 탭
4. 홈화면에 아이콘 생성됨

---

## 🔑 테스트 계정
| 역할 | 아이디 | 비밀번호 |
|------|--------|----------|
| 학생 | student | 1234 |
| 강사 | teacher | 1234 |
| 원장 | director | 1234 |

> 회원가입으로 새 계정을 만들 수도 있어요!

---

## ⚠️ 현재 버전 한계
- 데이터는 브라우저 localStorage에 저장됨 (기기별로 분리)
- 실시간 랭킹/멀티플레이 미지원
- Firebase 연동 시 실시간 동기화 가능

---

## 🔜 다음 단계 (선택사항)
- Firebase Firestore 연동 → 실시간 데이터 공유
- Firebase Auth 연동 → 소셜 로그인 (카카오, 구글)
- Firebase Hosting → 자체 도메인 (academy.brightfuture.kr)
