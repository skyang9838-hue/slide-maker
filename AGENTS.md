# Slide Maker Repository Instructions

슬라이드 이미지 생성, 수정, 재생성 또는 이어서 만들기 요청을 받으면 먼저 `WORKFLOW.md`, `STYLE_GUIDE.md`, `SLIDE_FORMAT.md`를 읽고 따릅니다.

## User-Facing Folders

- 모든 참고 파일은 종류를 나누도록 요구하지 말고 `넣을곳/`에서 확인합니다.
- 가장 최근 결과 이미지는 `결과물/` 바로 아래에 저장합니다.
- 새 전체 생성 전에 기존 결과 이미지를 `지난결과/<이전 실행 이름>/`으로 자동 보관합니다.
- 사용자에게 내부 작업 폴더를 직접 관리하도록 요구하지 않습니다.

## Internal Records

- 사용자가 붙여넣은 개요는 `.slide-maker/current-deck.md`에 저장합니다.
- 실행별 개요, 상태와 프롬프트는 `.slide-maker/runs/<실행 이름>/`에 기록합니다.
- 현재 실행 이름은 `.slide-maker/current-run.md`에 기록합니다.
- 실행 이름은 `YYYY-MM-DD_HHMM-short-title` 형식을 사용하고, 중복되면 `-02`, `-03`을 붙입니다.

## Reference Inference

- PPT 캡처, 예시 슬라이드와 무드보드는 스타일 참고 자료로 우선 판단합니다.
- 실제 사진은 `visual_type: provided_photo` 또는 사용자의 명시적인 요청이 있을 때만 사용합니다.
- 실제 사진이 없으면 사진풍 이미지를 생성하지 않고 편집 일러스트로 전환합니다.
- 로고와 제품 사진은 사용 목적과 배치 지시를 확인합니다.
- 파일의 용도가 결과에 큰 영향을 주면서 불분명할 때만 사용자에게 확인합니다.
- 참조 이미지 속 텍스트보다 개요의 사실 정보와 `required_text`를 우선합니다.

## Content And Visual Defaults

- 기본 시각 표현은 현대적인 편집 일러스트입니다.
- `visual_type`은 `illustration`, `diagram`, `typography`, `provided_photo` 중 하나로 해석합니다.
- 슬라이드에는 `headline`과 2~4개의 `key_phrases`를 기본으로 반영하고, `takeaway`가 있으면 함께 반영합니다.
- `key_phrases`를 단어 하나로 축약하거나 2개 미만으로 임의 삭제하지 않습니다.
- 이전 형식의 `title`, `draft_copy`, `visual_direction`은 새 필드로 정리한 뒤 생성합니다.

## Resume And Revision

- 특정 결과의 수정, 재생성 또는 이어서 만들기는 기존 결과와 내부 실행 기록을 사용합니다.
- 새로운 전체 생성 요청만 기존 `결과물/`을 보관하고 새 결과를 시작합니다.
