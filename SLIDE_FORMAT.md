# Slide Format

아래 형식은 웹 챗봇이 최종 슬라이드 개요를 정리할 때 사용하는 출력 양식입니다. 이 파일 전체를 웹 챗봇에 첨부하거나 복사해 붙여넣은 뒤, 지금까지 나눈 대화를 이 형식으로 정리해 달라고 요청하세요.

## 요청 문구 예시

```text
지금까지 나눈 발표 기획 내용을 아래 Markdown 형식에 맞춰 최종 정리해줘.
이 결과를 슬라이드 이미지 생성용 Codex에 전달할 거야.
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
- reference_style:
- reference_files:
- avoid:

## Content Rules

- must_keep:
- can_simplify:
- citation_or_source_notes:

## Slides

### Slide 01

- title:
- role:
- key_message:
- draft_copy:
- visual_direction:
- required_text:
- notes:

### Slide 02

- title:
- role:
- key_message:
- draft_copy:
- visual_direction:
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
- `reference_style`: 참고하고 싶은 디자인의 분위기와 특징을 글로 설명합니다.
- `reference_files`: `넣을곳/`에 넣은 파일명과 알고 있는 용도를 적습니다. 용도를 모르거나 Codex가 판단해도 된다면 파일명만 적어도 됩니다.
- `avoid`: 피해야 할 표현, 색, 분위기, 구성입니다.
- `must_keep`: 숫자, 날짜, 인명, 고유명사, 인용문처럼 바꾸면 안 되는 정보입니다.
- `can_simplify`: 길면 줄여도 되는 표현입니다.
- `citation_or_source_notes`: 출처 표기나 참고사항입니다.
- `role`: 표지, 문제 제기, 근거, 전환, 요약, 결론 등 해당 슬라이드의 역할입니다.
- `key_message`: 한 장에서 반드시 전달해야 하는 핵심 메시지입니다.
- `draft_copy`: 슬라이드에 들어갈 문구 초안입니다.
- `visual_direction`: 해당 슬라이드의 이미지 구성 아이디어입니다.
- `required_text`: 이미지 안에 반드시 정확히 들어가야 하는 문구입니다.
- `notes`: Codex가 참고할 추가 메모입니다.

## 작성 원칙

- 한 슬라이드에는 하나의 핵심 메시지만 둡니다.
- `draft_copy`는 길어도 괜찮지만, Codex가 이미지에 맞게 줄일 수 있습니다.
- `required_text`에 적힌 문구는 정확성을 우선합니다.
- 모르는 정보는 꾸며내지 말고 `미정`이라고 적습니다.
- 디자인 설명은 완벽할 필요가 없습니다. 원하는 분위기를 자연어로 적으면 됩니다.
- 예시 슬라이드, 로고와 사진은 구분하지 않고 모두 `넣을곳/`에 넣습니다.
- 참조 이미지 속 문구를 복사하지 말고, 실제 내용은 `required_text`와 `must_keep`을 기준으로 합니다.
