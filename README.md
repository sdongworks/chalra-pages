# chalra-pages

찰라(刹那) 앱의 공개 페이지. GitHub Pages로 서비스한다.

| 파일 | 주소 | 쓰이는 곳 |
|---|---|---|
| `privacy-policy.html` | https://sdongworks.github.io/chalra-pages/privacy-policy.html | 앱 설정 화면의 `개인정보처리방침`, Play Console 스토어 등록정보 |
| `app/index.html` | https://sdongworks.github.io/chalra-pages/app | 프로필·메신저에 넣는 짧은 주소. 꼬리표를 붙여 Play 스토어로 보낸다 |

## 고칠 때

- 방침을 바꾸면 **시행일**을 함께 고친다. 이전 시행일도 괄호로 남긴다.
- 앱이 처리하는 정보가 바뀌면(새 서비스 추가, 수집 항목 변경) 방침과 Play Console의
  **데이터 보안** 양식을 같이 고쳐야 한다.
- 배경과 초안은 앱 저장소의 `docs/monetization/PRIVACY_AND_DATA_SAFETY.md`에 있다.

## 짧은 주소 (`/app`)

자기소개란처럼 글자 수가 빠듯한 곳에 넣으려고 만들었다. 누르면 `referrer` 꼬리표가 붙은
Play 스토어 주소로 넘어간다.

유입 경로를 나눠 세려면 뒤에 `?s=이름`을 붙인다.

```
.../app              → utm_source=profile (기본값)
.../app?s=kakao      → utm_source=kakao
.../app?s=youtube    → utm_source=youtube
```

Play Console → 통계 → 획득 보고서의 트래픽 소스에서 나뉘어 보인다.

목적지를 바꿀 일이 생기면 이 파일만 고치면 된다. 프로필에 적어 둔 주소는 그대로 둔다.
