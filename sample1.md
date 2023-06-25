---
theme: seriph
layout: cover
background: "https://source.unsplash.com/1600x900/?nature,water"
fonts:
  sans: "Noto Sans CJK JP"
---

# Slidev

Hello, World!

---

# 目次

<Toc columns="2" />

---

# Page 2

<my-button m="t-4">
slot
<!-- <button @click="$slidev.nav.next">Next Page</button> -->
</my-button>
```html
<my-button>
<!-- <button @click="$slidev.nav.next">Next Page</button> -->
</my-button>
```
コードブロックを直接使用してハイライト表示する

```ts
console.log("Hello, World!");
```

---
layout: none
---

# Page 3

Windi CSS と Vue コンポーネントを直接使用して、スライドをスタイリングし、リッチにすることができます。

<div class="p-3">
  <Tweet id="1671161783401476096" />
</div>

---
layout: two-cols
---

<template v-slot:default>

# Left

</template>

<template v-slot:right>

# Right

</template>

---
layout: two-cols
---

# 左

左に配置される

::right::

# 右

右に配置される

---

# アニメーション

<!-- コンポーネントの使い方: "次へ"を押すまで、ここから下の内容は表示されません -->
<v-click>

Hello World

</v-click>

<!-- ディレクティブの使い方: 2回目の"次へ"を押すまで、ここから下の内容は表示されません -->
<div v-click class="text-xl p-2">

Hey!

</div>

---

# Components

<div grid="~ cols-2 gap-4">
<div>

You can use Vue components directly inside your slides.

We have provided a few built-in components like `<Tweet/>` and `<Youtube/>` that you can use directly. And adding your custom components is also super easy.

```html
<Counter :count="10" />
```

<!-- ./components/Counter.vue -->
<Counter :count="10" m="t-4" />

Check out [the guides](https://sli.dev/builtin/components.html) for more.

</div>
<div>

```html
<Tweet id="1390115482657726468" />
```

<Tweet id="1390115482657726468" scale="0.65" />

</div>
</div>

<!--
Presenter note with **bold**, *italic*, and ~~striked~~ text.

Also, HTML elements are valid:
<div class="flex w-full">
  <span style="flex-grow: 1;">Left content</span>
  <span>Right content</span>
</div>
-->



