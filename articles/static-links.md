---
layout: default
title: "Static Links"
date: 2026-11-06
---

I was building a compiler and I came across a problem. Consider this scenario in a compiled language:

```text
function foo() {
  local a = 69;
  function bar() {
    return a;
  }
}
```

### Frames
A compiled program has no environments to search. Each function call gets a block of memory on the stack called a *frame*.
