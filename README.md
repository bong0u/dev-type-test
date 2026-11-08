# 게임 개발자 유형 테스트

MBTI 16유형을 게임 개발 상황에 빗댄 재미용 테스트. 의존성 없는 단일 `index.html`.

## 배포 (GitHub Pages)
1. 새 저장소 생성 → `index.html`, `README.md` 업로드
2. Settings → Pages → Source: `Deploy from a branch`, Branch: `main` / `(root)`
3. 1~2분 후 `https://<계정>.github.io/<저장소>/` 에서 확인

## 구조
- `QUESTIONS` : 12문항 (E/I, S/N, T/F, J/P 축당 3개). 각 선택지의 `v`가 해당 축 글자로 가산
- `TYPES` : 16유형 결과 데이터 (이름·캐치프레이즈·태그·행동·강점·주의·찰떡/티격태격·포지션)
- 결과 URL : `?r=INTJ` 형태. 공유 링크로 진입 시 바로 결과 화면 표시
- 공유 : 모바일은 네이티브 공유 시트(`navigator.share`), PC는 클립보드 복사

## 수정 포인트
- 유형명/카피 변경 → `TYPES`의 `name`, `catch`, `tags` 등
- 문항 수정 → `QUESTIONS` (축별 개수는 홀수 유지 권장: 동점 방지)
- 일러스트 추가 → 결과 화면 `#rEmoji` 자리를 `<img>`로 교체
- OG 이미지 → `<head>`에 `og:image` 추가 (공유 썸네일)
