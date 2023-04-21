---
title: "Проба пера"
date: "2021-09-11"
draft: true
categories: ["other"]
tags: ["intro"]
---

Первая запись за столько лет

1. Перед этим будет много текста. 1.
2. Перед этим будет много текста. 2.
3. Перед этим будет много текста. 3.
4. Перед этим будет много текста. 4.
5. Перед этим будет много текста. 5.
6. Перед этим будет много текста. 6.
7. Перед этим будет много текста. 7.
8. Перед этим будет много текста. 8.
9. Перед этим будет много текста. 9.

Окончание проверочного текста. Тем самым мы заершаем преамбулу на начальной странице.

Пример подцветки кода.

{{< highlight c "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char **argv) {
  return EXIT_SUCCESS;
}
{{< / highlight >}}

Таблица

{{< pure_table
  "Колонка №1|Колонка №2|Колонка №3"
  "Данные 1.1|Данные 1.2|Данные 1.3"
  "Данные 2.1|Данные 2.2|Данные 2.3"
  "Данные 3.1|Данные 3.2|Данные 3.3"
>}}

Диаграмма

{{< plantuml id="eg" >}}
participant participant as Foo
actor       actor       as Foo1
boundary    boundary    as Foo2
control     control     as Foo3
entity      entity      as Foo4
database    database    as Foo5
collections collections as Foo6
queue       queue       as Foo7
Foo -> Foo1 : To actor 
Foo -> Foo2 : To boundary
Foo -> Foo3 : To control
Foo -> Foo4 : To entity
Foo -> Foo5 : To database
Foo -> Foo6 : To collections
Foo -> Foo7: To queue
{{< /plantuml >}}

{{< mermaid >}}
stateDiagram-v2
  open: Open Door
  closed: Closed Door
  locked: Locked Door
  open   --> closed: Close
  closed --> locked: Lock
  locked --> closed: Unlock
  closed --> open: Open
{{< /mermaid >}}

```dot {style=xkcd}
digraph graphname {
  splines="curved";
  a -> b -> c;
  b -> d -> a;
}
```

Изображение

{{< figure src="https://dburet.gitlab.io/img/2021/04/rust-and-fractals.png" title="Fractal" >}}

Gist

{{< gist Pastor 46186fee205bdfae4895a2b8e4cbc33f >}}

References

https://gohugo.io/content-management/shortcodes
[Who]({{< relref "about.md#who" >}})

Mathematics

$$f(x) = sin(x) + 12$$

{{< mathjax >}}
$$
\begin{vmatrix}a & b\\
c & d
\end{vmatrix}
$$
{{< /mathjax >}}
