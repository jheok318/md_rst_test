# RST, MD

- RST : reStructuredText
- MD :  Markdown
- index.rst : 웹 문서의 첫 페이지

## RST

### 헤더

- 헤더의 위/아래에 들어가는 문자의 갯수는 헤더내용과 같거나 많아야 한다.

```rst
# 잘못된 예
title
==

# 잘된 예
title
=====

title
=======
```

- 헤더 레벨은 정해진 규칙은 없다.
- 하지만, 하나의 프로젝트에는 `#, *, =, -, ^, ",`' 같은 특수 문자를 이용해 헤더 레벨을 정의 하여 쓰는 것이 좋다.

```rst
 #RST                   # MarkDown

==============
Section Title           # Section Title
==============

--------------
Section Title           ## Section Title
--------------

Section Title           ### Section Title
=============

Section Title           #### Section Title
-------------

Section Title           ##### Section Title
\`````````````

Section Title           ###### Section Title
'''''''''''''
```

### 목록

- #. 은 번호 자동생성

```rst
1. 목록
2. 목록
#. 목록
```

### 들여쓰기

```rst
들여쓰기 없음
    띄어쓰기 4번 들여쓰기 1번
        띄어쓰기 8번 들여쓰기 2번
    띄어쓰기 4번 들여쓰기 1번
들여쓰기 없음
```

### 코드블록

- Markdown의 ```라고 생각하면 된다.

```c
.. code::

printf_s("rst");
```

### 이미지

```
.. image:: 이미지파일 경로
	:height: 250
	:width: 250
	:scale: 50
	:alt: 이미지 설명
```

### 표

- 표를 표현하는 방식은 2가지이다.

```
+------------+------------+-----------+ 
| Header 1   | Header 2   | Header 3  | 
+============+============+===========+ 
| body row 1 | column 2   | column 3  | 
+------------+------------+-----------+ 
| body row 2 | Cells may span columns.| 
+------------+------------+-----------+ 
| body row 3 | Cells may  | - Cells   | 
+------------+ span rows. | - contain | 
| body row 4 |            | - blocks. | 
+------------+------------+-----------+

=====  =====  ====== 
   Inputs     Output 
------------  ------ 
  A      B    A or B 
=====  =====  ====== 
False  False  False 
True   False  True 
False  True   True 
True   True   True 
=====  =====  ======
```

### 수평선

- 단락 분리시 사용
- 4개 이상의 -를 사용하여 표시
- 위 아래 줄에 어떠한 문자가 있어서는 안됨

```
ABCDEF

--------

GHIJKL
```

### 하이퍼링크

```
.. _링크1: http://www.naver.com/

'링크2 <http://www.naver.com/>'_
```