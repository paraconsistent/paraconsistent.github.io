---
layout: post
math: "true"
toc: "true"
title: 편집기 팁
categories: Coding
tags:
  - tips
---
# 편집기 팁

특정 편집기 보다는 일반적으로 통용되는 내용로 작성하였다.

## 이동과 편집

### 기본 커서 이동키

| 키               | 식별자   | 기능           |
| --------------- | ----- | ------------ |
| <kbd>←</kbd>    | Left  | 좌측으로 한 문자 이동 |
| <kbd>→</kbd>    | Right | 우측으로 한 문자 이동 |
| <kbd>↑</kbd>    | Up    | 위로 한 줄 이동    |
| <kbd>↓</kbd>    | Down  | 아래로 한 줄 이동   |
| <kbd>Home</kbd> | Home  | 줄의 시작으로 이동   |
| <kbd>End</kbd>  | End   | 줄의 끝으로 이동    |
| <kbd>PgUp</kbd> | PgUp  | 페이지의 시작으로 이동 |
| <kbd>PgDn</kbd> | PgDn  | 페이지의 끝으로 이동  |

### 기본 편집키

| 키                    | 식별자               | 기능           |
| -------------------- | ----------------- | ------------ |
| <kbd>Space</kbd>     | Space             | 띄어쓰기         |
| <kbd>Enter</kbd>     | Enter, Return, CR | 줄 바꿈         |
| <kbd>Tab</kbd>       | Tab               | 들여쓰기         |
| <kbd>Backspace</kbd> | Backspace         | 뒤로 한 문자 지우기  |
| <kbd>Ins</kbd>       | Ins               | 삽입/수정 모드 전환  |
| <kbd>Del</kbd>       | Del               | 앞으로 한 문자 지우기 |
| <kbd>Caps Lock</kbd> | Caps Lock         |              |

### 조합키

| 키                | 식별자       | 기능                 | 비고                                                        |
| ---------------- | --------- | ------------------ | --------------------------------------------------------- |
| <kbd>Ctrl</kbd>  | Ctrl, C-  | 한 묶음 단위로 수행        | 한 묶음의 단위는 프로그램마다 다르지만, 일반적으로 한 단어(즉, 하나의 연속된 알파벳과 숫자의 나열) |
| <kbd>Shift</kbd> | Shift, S- | 선택, 반대로 수행         | 반대 명령의 단축키는 보통 원래 명령어 단축키에서  <kbd>⇧ Shift</kbd>와 조합하는 형태  |
| <kbd>Alt</kbd>   | Alt       | 해당 알파벳에 해당하는 패널 선택 | 일반적으로 <kbd>Alt</kbd>를 꾹 누르면 눌러야 하는 키가 밑줄 쳐짐               |

| 이동/편집 조합                                      | 기능            | 비고         |
| --------------------------------------------- | ------------- | ---------- |
| <kbd>Ctrl</kbd>+<kbd>←</kbd>                  | 왼쪽으로 한 단어 이동  |            |
| <kbd>Ctrl</kbd>+<kbd>→</kbd>                  | 오른쪽으로 한 단어 이동 |            |
| <kbd>Ctrl</kbd>+<kbd>↑</kbd>                  | 위로 한 단위 이동    | 프로그램 마다 다름 |
| <kbd>Ctrl</kbd>+<kbd>↓</kbd>                  | 아래로 한 단위 이동   | 프로그램 마다 다름 |
| <kbd>Ctrl</kbd>+<kbd>A</kbd>                  | 문서 전체 선택      |            |
| <kbd>Ctrl</kbd>+<kbd>Z</kbd>                  | 실행 취소         |            |
| <kbd>Ctrl</kbd>+<kbd>X</kbd>                  | 잘라내기          |            |
| <kbd>Ctrl</kbd>+<kbd>C</kbd>                  | 복사            |            |
| <kbd>Ctrl</kbd>+<kbd>V</kbd>                  | 붙여넣기          |            |
| <kbd>Ctrl</kbd>+<kbd>Home</kbd>               | 문서 시작으로 이동    |            |
| <kbd>Ctrl</kbd>+<kbd>End</kbd>                | 문서 끝으로 이동     |            |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>Z</kbd> | 다시 실행         |            |
| <kbd>Ctrl</kbd>+<kbd>Ins</kbd>                | 복사            |            |
| <kbd>Shift</kbd>+<kbd>Ins</kbd>               | 붙여넣기          |            |

| 편집기 조합                                        | 기능                            | 비고                                    |
| --------------------------------------------- | ----------------------------- | ------------------------------------- |
| <kbd>Ctrl</kbd>+<kbd>F</kbd>                  | 찾기                            |                                       |
| <kbd>Ctrl</kbd>+<kbd>R</kbd>                  | 찾아 바꾸기                        |                                       |
| <kbd>Ctrl</kbd>+<kbd>W</kbd>                  | 현재 창 종료                       |                                       |
| <kbd>Ctrl</kbd>+숫자                            | 왼쪽으로부터 해당 숫자에 해당하는 위치의 탭으로 이동 | 예: <kbd>Ctrl</kbd>+<kbd>1</kbd>은 첫째 탭 |
| <kbd>Ctrl</kbd>+<kbd>Tab</kbd>                | 오른쪽 탭으로 순환 이동                 |                                       |
| <kbd>Shift</kbd>+<kbd>Tab</kbd>               | 왼쪽 탭으로 순환 이동                  |                                       |
| <kbd>Ctrl</kbd>+<kbd>N</kbd>                  | 새로 만들기                        |                                       |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>N</kbd> | 새 창                           |                                       |
| <kbd>Ctrl</kbd>+<kbd>O</kbd>                  | 열기                            |                                       |
| <kbd>Ctrl</kbd>+<kbd>S</kbd>                  | 저장                            |                                       |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>S</kbd> | 다른 이름으로 저장                    |                                       |
| <kbd>Ctrl</kbd>+<kbd>+</kbd>                  | 확대                            |                                       |
| <kbd>Ctrl</kbd>+<kbd>-</kbd>                  | 축소                            |                                       |
| <kbd>F1</kbd>                                 | 도움말                           | 가장 중요하다!                              |
| <kbd>Alt</kbd>+<kbd>F4</kbd>                  | 종료                            |                                       |
