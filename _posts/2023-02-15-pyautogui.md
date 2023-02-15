---
layout: post
title: pyautogui 마우스 자동화 기본 사용법
date: 2023-02-15 10:00:00 +0900
category: python
---

### 라이브러리 설치

```bat
pip install pyautogui
```

<br>

### size:모니터 해상도 사이즈 출력

```python
print(pyautogui.size())
```

<br>

### position:현재 마우스 위치 출력

```python
print(pyautogui.position())
```

<br>

### moveTo:원하는 좌표로 마우스 이동

```python
# x 300, y 300의 좌표로 마우스 즉시 이동
pyautogui.moveTo(300, 300)

# x 300, y 300의 좌표로 마우스를 10초간 이동
pyautogui.moveTo(300, 300, 10)
```

<br>

### click:마우스 클릭하기

```python
pyautogui.click() # 좌클릭
pyautogui.click(button='right') # 우클릭
pyautogui.doubleClick() # 더블클릭
pyautogui.click(click = 10, interval = 1) # 1초 간격으로 10번 클릭
```

<br>

### dragTo:마우스 드래그하기

```python
pyautogui.moveTo(300, 300)
pyautogui.dragTo(500, 500, 2)
```
