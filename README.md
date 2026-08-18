# Dameum.github.io

더담음(TheDameum) 공식 사이트.

## 구조

```
.
├── index.html                        https://TheDameum.github.io/
├── app-ads.txt                       https://TheDameum.github.io/app-ads.txt
└── tap-pop-ai/
    └── privacy/
        └── index.html                https://TheDameum.github.io/tap-pop-ai/privacy/
```

## 주요 URL

| 용도 | URL | 쓰이는 곳 |
|---|---|---|
| 개인정보처리방침 | `https://TheDameum.github.io/tap-pop-ai/privacy/` | Play Console > 앱 콘텐츠 |
| 개발자 웹사이트 | `https://TheDameum.github.io/` | Play Console > 스토어 등록정보 |
| app-ads.txt | `https://TheDameum.github.io/app-ads.txt` | AdMob 광고 단가 인증 |

## app-ads.txt 확인 사항

현재 내용은 AdMob 게시자 ID(`pub-7249515779843261`) 기준으로 작성된 표준 형식입니다.

```
google.com, pub-7249515779843261, DIRECT, f08c47fec0942fa0
```

⚠️ **AdMob 콘솔 > 앱 > app-ads.txt에서 제공하는 줄과 대조해 확인하세요.** 미디에이션 네트워크를 추가하면 줄이 더 늘어납니다.
AdMob이 이 파일을 크롤링하려면 Play Console 스토어 등록정보에 개발자 웹사이트 URL이 등록되어 있어야 합니다.

## 새 앱을 추가할 때

앱마다 디렉터리를 하나 만들고 그 아래 `privacy/index.html`을 둡니다.

```
├── tap-pop-ai/privacy/index.html
└── <새-앱-이름>/privacy/index.html
```

이렇게 하면 기존 URL이 절대 깨지지 않습니다. **Play Console에 등록한 개인정보처리방침 URL이 404가 되면 정책 위반**이므로, 한 번 등록한 경로는 바꾸지 마세요.

## 배포

`main` 브랜치에 push하면 GitHub Pages가 자동 배포합니다 (Settings > Pages > Deploy from a branch > main / root).
반영까지 보통 1~2분 걸립니다.
