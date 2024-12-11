---
id: my-doc-id
title: My document title
description: My document description
slug: /my-custom-url
---

export const Highlight = ({children, color}) => (
  <span
    style={{
      backgroundColor: color,
      borderRadius: '20px',
      color: '#fff',
      padding: '10px',
      cursor: 'pointer',
    }}
    onClick={() => {
      alert(`You clicked the color ${color} with label ${children}`)
    }}>
    {children}
  </span>
);

## Markdown heading

Markdown text with [links](./hello.md)

to [mogemoge](./mogemoge)

to [create a page](./tutorial-basics/create-a-page)

```js
console.log('Hello, world!');
const hoge = () => {
  console.log('hoge');
  return 'hoge';
}
```

:::tip[My tip]

Use this awesome feature option

:::

:::danger[Take care]

This action is dangerous

:::

This is <Highlight color="#25c2a0">Docusaurus green</Highlight> !

This is <Highlight color="#1877F2">Facebook blue</Highlight> !

![](/img/undraw_docusaurus_mountain.svg)
