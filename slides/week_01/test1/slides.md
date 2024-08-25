---
title: Test
layout: cover
theme: neversink
color: bowdoin
routerMode: hash
addons:
  - slidev-addon-excalidraw
---

# Test
This is a _test_ of ==neversink== with a **custom** color scheme!  

I hope this works?

---
title: Test
layout: side-title
titlewidth: is-4
align : rm-cm
theme: neversink
color: bowdoin-title
---

:: title ::

# Check out these slides yourself!

:: content ::

<QRCode value="https://christopherwmm.github.io/lectures/week_01/test1/" :size="300" render-as="svg" />

---
title: Test
layout: side-title
titlewidth: is-3
align : rm-lm
theme: neversink
color: bowdoin-title
---

:: title ::

# Code!

:: content ::

## We can execute some `code`!

```ts {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
console.log("Hello world!")
```

---
layout: top-title-two-cols
align : l-lm-c
theme: neversink
color: bowdoin-title
---

:: title ::

# This has a list of things and a drawing

:: left ::

- A
  + a
  + aa
- B
- C

:: right ::

<Excalidraw drawFilePath="./test.excalidraw" />