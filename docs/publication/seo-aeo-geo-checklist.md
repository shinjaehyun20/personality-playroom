# 공개 웹사이트 SEO · AEO · GEO 게이트

이 프로젝트는 공개 전 아래 게이트를 통과한다. **검색 노출·AI 인용·순위는 보장하지 않는다.** 목적은 정확하게 이해되고 공유될 수 있는 정본 표면을 만드는 것이다.

## 1. SEO — 검색 엔진이 페이지를 식별할 수 있는가
- [ ] 페이지별 고유 `<title>` (주제 + 사용자 효용)
- [ ] 110~160자 내의 고유 meta description
- [ ] canonical URL 1개, HTTPS 최종 URL과 일치
- [ ] `robots.txt`가 sitemap URL을 가리킴
- [ ] 유효한 `sitemap.xml`의 URL이 canonical과 일치
- [ ] 404·비공개·로그인 페이지를 sitemap에 넣지 않음

## 2. 공유/OG — 링크 하나만으로 클릭 이유가 보이는가
- [ ] `og:title`, `og:description`, `og:url`, `og:image`, `og:image:alt`
- [ ] X Card의 title/description/image/alt
- [ ] OG 이미지는 1200×630, 한글 제목·CTA·핵심 비주얼이 잘리지 않음
- [ ] 실제 원격 HTML과 이미지 URL을 다시 읽음

## 3. AEO — 질문에 바로 답할 수 있는가
- [ ] 첫 화면/README에 `무엇을 하는가`, `누구에게 유용한가`, `어떻게 쓰는가`가 명확함
- [ ] 제한·비보장·안전 경계가 본문에 있음
- [ ] 질문형 헤딩 또는 FAQ가 실제 사용자의 질문을 답함
- [ ] 구조화 데이터는 보이는 본문과 모순되지 않음

## 4. GEO — AI가 잘못 설명하지 않도록 정본을 주는가
- [ ] JSON-LD의 type/name/description/url/image/author가 정확함
- [ ] 과장된 수치·희귀도·성능·의학/심리 주장을 넣지 않음
- [ ] GitHub About, README, 라이브 페이지의 핵심 설명이 동일함
- [ ] 변경 후 검색/AI 노출 성과는 측정 항목으로만 기록; 즉시 반영으로 주장하지 않음

## 5. 배포 후 재검증
1. 원격 HTML에서 title·canonical·OG·JSON-LD를 파싱한다.
2. `robots.txt`, `sitemap.xml`, OG 이미지가 200인지 확인한다.
3. 모바일 390px와 데스크톱에서 텍스트 잘림·가로 스크롤·콘솔 오류를 확인한다.
4. 링크 공유 이미지는 플랫폼 캐시가 남을 수 있으므로 URL 변경/캐시 새로고침 여부를 별도 기록한다.

## 현재 적용
- 대상: 선택코드 플레이룸
- 기준 URL: https://shinjaehyun20.github.io/personality-playroom/
- 검증기: `D:/workspace/tools/stack/verify_public_web_visibility.py`
