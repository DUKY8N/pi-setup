---
name: commit-message
description: Git 커밋 메시지 작성에 사용한다. 저장소 관례를 우선하고, 없으면 영어 Conventional Commits를 따른다.
---

# Commit Message

## 관례 확인

1. `git log -20 --format=%s`로 최근 커밋 제목을 확인한다.
2. 언어, 형식, type, scope, 대소문자 등 일관된 관례가 있으면 그대로 따른다.
3. 관례가 없거나 일관되지 않으면 영어로 [Conventional Commits 1.0.0](references/conventional-commits-v1.0.0.md)을 따른다.

## 변경사항 확인

1. 사용자가 변경사항을 제공했다면 그것을 우선한다.
2. 없다면 `git diff --cached`를 확인한다.
3. staged 변경이 없다면 `git diff`와 `git status --short`를 확인한다.
4. 변경사항이 없거나 의도가 불명확하면 추측하지 말고 짧게 질문한다.

## 출력

가장 적합한 메시지 하나를 복사 가능한 코드 블록으로 제시한다.
