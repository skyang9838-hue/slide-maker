# Slide Format

아래 형식은 웹 챗봇이 최종 슬라이드 개요를 정리할 때 사용하는 출력 양식입니다. 이 파일 전체를 웹 챗봇에 첨부하거나 복사해 붙여넣은 뒤, 지금까지 나눈 대화를 이 형식으로 정리해 달라고 요청하세요.

## 요청 문구 예시

```text
지금까지 나눈 발표 기획 내용을 아래 Markdown 형식에 맞춰 최종 정리해줘.
이 결과를 슬라이드 이미지 생성용 Codex에 전달할 거야.
각 슬라이드에는 제목과 함께 2~4개의 짧은 핵심 구절을 작성해줘.
설명문이나 발표 대본처럼 길게 쓰지 말고, 단어 하나보다 의미가 분명한 짧은 구절로 써줘.
사실, 숫자, 날짜, 인명, 고유명사는 임의로 바꾸지 말고, 모르는 내용은 비워두거나 "미정"이라고 써줘.
```

## 출력 형식

```markdown
# Deck Brief

## Project

- title:
- audience:
- purpose:
- desired_slide_count:
- language:
- aspect_ratio: 16:9
- output_type: finished slide images

## Style

- overall_mood:
- visual_keywords:
- color_direction:
- typography_direction:
- default_visual_medium: editorial_illustration
- illustration_style:
- photo_policy: provided_only
- reference_style:
- reference_files:
- avoid:

## Content Rules

- must_keep:
- can_simplify:
- citation_or_source_notes:

## Slides

### Slide 01

- headline:
- role:
- key_message:
- key_phrases:
  -
  -
  -
- takeaway:
- visual_type: illustration
- visual_subject:
- composition:
- required_text:
- notes:

### Slide 02

- headline:
- role:
- key_message:
- key_phrases:
  -
  -
- takeaway:
- visual_type: diagram
- visual_subject:
- composition:
- required_text:
- notes:
```

## 필드 설명

- `title`: 전체 발표 또는 콘텐츠 제목입니다.
- `audience`: 슬라이드를 보는 대상입니다.
- `purpose`: 설득, 교육, 보고, 소개 등 발표 목적입니다.
- `desired_slide_count`: 원하는 슬라이드 수입니다.
- `language`: 슬라이드 안에 들어갈 언어입니다.
- `aspect_ratio`: 기본값은 `16:9`입니다.
- `overall_mood`: 전체 분위기입니다.
- `visual_keywords`: 예: 미니멀, 잡지형, 친근함, 고급스러움.
- `color_direction`: 색상 방향입니다.
- `typography_direction`: 글꼴과 타이포그래피 느낌입니다.
- `default_visual_medium`: 별도 지정이 없을 때 `editorial_illustration`을 사용합니다.
- `illustration_style`: 선, 질감, 인물 표현과 색상 등 전체 일러스트 방향입니다.
- `photo_policy`: 기본값은 `provided_only`입니다. 사용자가 제공한 실제 사진만 사용한다는 뜻입니다.
- `reference_style`: 참고하고 싶은 디자인의 분위기와 특징을 글로 설명합니다.
- `reference_files`: `넣을곳/`에 넣은 파일명과 알고 있는 용도를 적습니다. 용도를 모르거나 Codex가 판단해도 된다면 파일명만 적어도 됩니다.
- `avoid`: 피해야 할 표현, 색, 분위기, 구성입니다.
- `must_keep`: 숫자, 날짜, 인명, 고유명사, 인용문처럼 바꾸면 안 되는 정보입니다.
- `can_simplify`: 길면 줄여도 되는 표현입니다.
- `citation_or_source_notes`: 출처 표기나 참고사항입니다.
- `headline`: 슬라이드 화면에 들어갈 제목입니다.
- `role`: 표지, 문제 제기, 근거, 전환, 요약, 결론 등 해당 슬라이드의 역할입니다.
- `key_message`: 한 장에서 반드시 전달해야 하는 의미입니다. 화면 문구가 아니라 제작 기준입니다.
- `key_phrases`: 화면에 넣을 2~4개의 짧은 핵심 구절입니다.
- `takeaway`: 발표 후 기억에 남겨야 할 한 문구입니다. 필요하지 않으면 비워도 됩니다.
- `visual_type`: `illustration`, `diagram`, `typography`, `provided_photo` 중 하나를 사용합니다. 비어 있으면 `illustration`입니다.
- `visual_subject`: 일러스트, 다이어그램 또는 사진으로 보여줄 대상입니다.
- `composition`: 화면 배치와 시선 흐름을 간단히 적습니다.
- `required_text`: 철자까지 정확해야 하는 필수 문구입니다. `headline`, `key_phrases`, `takeaway`와 중복되어도 됩니다.
- `notes`: Codex가 참고할 추가 메모입니다.

## 핵심 구절 작성 원칙

- `key_phrases`는 슬라이드마다 2~4개를 권장합니다.
- 각 구절은 한국어 기준 약 10~20자 안팎으로 작성합니다.
- 발표 대본 같은 완전한 문장보다 명사형이나 짧은 서술형을 사용합니다.
- `고민`, `성장`처럼 단어 하나만 나열하지 말고 `처음이라 더 깊어진 고민`처럼 의미가 드러나게 씁니다.
- 구절 끝에는 특별한 이유가 없으면 마침표를 붙이지 않습니다.
- 화면이 복잡해지면 구절의 표현을 다듬을 수 있지만, 2개 미만으로 임의 삭제하지 않습니다.

## 시각 유형 원칙

- `illustration`: 기본값입니다. 현대적인 편집 일러스트와 잡지 삽화 느낌을 사용합니다.
- `diagram`: 과정, 흐름, 비교, 구조와 수치 관계를 보여줄 때 사용합니다.
- `typography`: 강한 전환 문구나 결론처럼 글자 자체가 화면의 중심일 때 사용합니다.
- `provided_photo`: `넣을곳/`에 실제 사용할 사진이 있을 때만 사용합니다.
- 실제 사진이 없으면 비슷한 현장 사진을 새로 만들어 대체하지 않고 `illustration`이나 `diagram`으로 전환합니다.

## 작성 원칙

- 한 슬라이드에는 하나의 핵심 메시지만 둡니다.
- 기본 화면 정보량은 `headline` 1개, `key_phrases` 2~4개, 선택적인 `takeaway` 1개입니다.
- `required_text`에 적힌 문구는 정확성을 우선합니다.
- 모르는 정보는 꾸며내지 말고 `미정`이라고 적습니다.
- 예시 슬라이드, 로고와 사진은 구분하지 않고 모두 `넣을곳/`에 넣습니다.
- 참고 PPT 이미지는 스타일만 참고하고, 실제 사진은 사용 목적이 명시된 경우에만 결과에 사용합니다.
- 참조 이미지 속 문구를 복사하지 말고 실제 내용은 개요의 필드를 기준으로 합니다.

## 이전 형식 호환

기존 개요에 `title`, `draft_copy`, `visual_direction`이 있으면 Codex가 의미를 보존해 `headline`, `key_phrases`, `visual_subject`, `composition`으로 정리한 뒤 생성할 수 있습니다. 새 개요에는 위의 새 필드를 사용합니다.
