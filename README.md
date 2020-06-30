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

```rst
들여쓰기 없음
    띄어쓰기 4번 들여쓰기 1번
        띄어쓰기 8번 들여쓰기 2번
    띄어쓰기 4번 들여쓰기 1번
들여쓰기 없음
```

