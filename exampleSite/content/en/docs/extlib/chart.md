---
title: lala
date:
description:
libraries:
- chart
- flowchartjs
- katex
---

chart

```chart
{
    "type": "bar",
    "data": 
       {
        "labels": ["One", "Two", "Three", "Four", "Five", "Six"],
        "datasets": [{
            "label": "# of Votes",
            "data": [12, 19, 3, 5, 3, 8]
        }]
    }
}
```

```chart
    {
    "type": "line",
        "data": {
            "labels": ["One", "Two", "Three", "Four", "Five", "Six"],
            "datasets": [
            {
                "label": "# of Votes",
                "data": [12, 19, 3, 5, 2, 3],
                "backgroundColor":"transparent",
                "borderColor":"orange"
            },
            {
                "label": "Some other set",
                "data": [15, 8, 13, 5, 5, 9],
                "backgroundColor":"transparent",
                "borderColor":"#44ccff"
            }
            ]
        }
    }
```

flowchartjs

```flowchart
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End|future:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|future

st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e
```

katex

The following

$$ \int_{a}^{b} x^2 dx $$

Is an integral

$$ \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } $$

Enable Katex in the config file by setting the `katex` param to `true`. This will import the necessary Katex CSS/JS. 

See the online reference of [supported TeX functions](https://katex.org/docs/supported.html). 

**Note:** For inline math to render correctly, your content file extension must be `.mmark`. See the [official mmark site](https://mmark.nl/). 

```
Inline math: $ \varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887… $
```

Inline math: $ \varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887… $

```
Block math:

$$ \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } $$
```

Block math:

$$ \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } $$
