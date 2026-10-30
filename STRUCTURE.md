# STRUCTURE · rollday-sample

```
rollday-sample/
├─ index.html              단일 파일 (CSS·JS 인라인, lang="en")
├─ wrangler.toml           name = rollday-sample → rollday-sample.lgt3232.workers.dev (폴더명 = name, 배포 이름도 같게)
├─ .assetsignore           img/ · 문서 · index_*.html · _deploy 배포 제외
├─ rd-grandstander.woff2   제목 · 워드마크 (Grandstander 600–800, 라틴만)
├─ rd-pretendard.woff2     본문 · 한글 (Pretendard 400–700)
├─ rd-logo.webp            초록 원 + 토끼 + Roll Day 투명 로고 (스토리)
├─ rd-mark.webp            원 마크만 (헤더 · 히어로 배지) · favicon.png
├─ rd-hero.webp            히어로 오븐 팬 시나몬롤
├─ rd-roll-*.webp          The rolls 6장
├─ rd-bake / rd-case / rd-shop .webp   Our promise 아래 3장
├─ rd-box.webp             To go
├─ og-rollday.jpg
├─ img/                    다올 제공 원본 52장 (배포 제외 · 사람 · 타 브랜드 로고 포함, 레포에 올리지 말 것)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더 → 히어로(베이지) → `#story`(흰) → `#rolls`(베이지) → `#promise`(초록) → To go(흰) → `#visit`(베이지) → 푸터(초록) + 모바일 `.quick`.

## 영업시간 수정 (4곳)
히어로 `.when` · Visit `.hours` 표 · 푸터 · head JSON-LD.

## 폰트 재생성
문구를 바꾸면 빠진 글자 검사(LESSONS §26). Grandstander는 instancer로 wght 600–800 고정 후 라틴 글자만 서브셋 · `--name-IDs='*' --name-languages='*' --name-legacy`(§24).
