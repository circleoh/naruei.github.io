---
layout: post
title:  Recursion
tags: PL
open: true
mathjax: on
---

### Recursive functions

Let's define a simple recursive function, which computes the sum from $0$ to $n$.
`func sum(_ x: Int) -> Int {
    if (x == 0) { 
        return 0
    }
    else {
        return (x + sum(x - 1))
    }
}`
$$ \frac{\sigma \vdash e_1 \implies 0 \qquad \sigma \vdash e_2 \implies v}{\sigma \vdash \texttt{if0} \, e_1 \, e_2 \, e_3 \implies v} $$

The following `code` implements this idea.
```
import math

for i in range(10):
    print("this is wrong!")
```

*All the materials are from CS320 class held on KAIST.*