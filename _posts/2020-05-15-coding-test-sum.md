---
title: "Coding Test: 두 정수 사이의 합"
date: 2020-05-15
header:
  # teaser: /assets/images/coding-test/gamestar.png
  # og_image: /assets/images/page-header-teaser.png
categories:
  - coding test
  - python
tags:
  - level 1
published: true
---

### 두 정수 사이의 합

---

#### 문제 설명

두 정수 a, b가 주어졌을 때 a와 b 사이에 속한 모든 정수의 합을 리턴하는 함수, solution을 완성하세요.
예를 들어 a = 3, b = 5인 경우, 3 + 4 + 5 = 12이므로 12를 리턴합니다.

#### 제한사항

- a와 b가 같은 경우는 둘 중 아무 수나 리턴하세요.
- a와 b는 -10,000,000 이상 10,000,000 이하인 정수입니다.
- a와 b의 대소관계는 정해져있지 않습니다.

#### 입출력 예

| 3 | 5 | 12 |
| 3 | 3 | 3 |
| 5 | 3 | 12 |

---

```python
def solution(a, b):
    answer = 0

    if a <= b:
        for i in range(a,b+1):
            answer += i
    else:
        for i in range(b,a+1):
            answer += i

    return answer
```

간단한 조건문으로 풀이.
