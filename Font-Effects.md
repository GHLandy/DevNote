# 文字效果

## 模糊文字

```css
/* 文字包含在 elem 元素中 */
elem {
  color: transparent;
  -ms-text-shadow: 0 0 5px #1db910;
  text-shadow: 0 0 5px #1db910;
}
```

## 镂空文字

```css
/* 文字包含在 elem 元素中 */
elem {
  color: transparent;
  -webkit-text-stroke: 2px #1db910;
}
```

## 渐变、图片背景文字

```css
/* 文字包含在 elem 元素中 */
elem {
  color: transparent;
  background: linear-gradient(to right, #1db910 0%, #54d0a7 50%, #299ad1 100%);
  -webkit-background-clip: text;
  background-clip: text;
}
```
