---
layout:     post
title:      "CSS select except last child"
subtitle:   "마지막 자식 노드를 제외한 선택자"
date:       2018-10-05
author:     "Jonghun Park"
header-img: "img/post-bg-css.jpg"
header-mask: 0.3
catalog:    true
tags:
  - web
  - css
---

## 마지막 Child 제외하기

마지막 Child 를 제외하고서, 다른 것들에 대해서만 특정 CSS를 적용해야 하는 경우 아래와 같은 CSS Selector를 사용하면 됩니다. :not() 은 ()안의 조건이 아닌 :앞의 tag를 선택하라는 것이고, :last-child 는 마지막 child 라는 것이므로, 마지막 child 를 제외한 나머지를 선택하는 selector가 됩니다.

```css
ul li:not(:last-child)
```

출처: https://4urdev.tistory.com/51 [Simplify]