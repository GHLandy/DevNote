# 文字特效

> First Create: 2017-10-28 GHLandy (GHLandy@GHLandy.com)
>
> Last Upate: 2017-11-28 GHLandy (GHLandy@GHLandy.com)

## 模糊文字

```css
/* 文字包含在 elem 元素中 */
elem {
  color: transparent;
  -ms-text-shadow: 0 0 5px #1db910;
  text-shadow: 0 0 5px #1db910;
}
```

> Google Chrome 62.0.3202.62、Mozilla Firefox 57.0b10 支持 text-shadow
>
> Microsoft IE 11、Microsoft Edge 40.15063.674.0 不支持

## 镂空文字

```css
/* 文字包含在 elem 元素中 */
elem {
  color: transparent;
  -webkit-text-stroke: 2px #1db910;
}
```

> Google Chrome 62.0.3202.62、Mozilla Firefox 57.0b10、Microsoft Edge 40.15063.674.0 支持 -webkit-text-stroke
>
> Microsoft IE 11 不支持

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

> Google Chrome 62.0.3202.62 支持 -webkit-background-clip
>
> Mozilla Firefox 57.0b10、Microsoft Edge 40.15063.674.0 支持 background-clip
>
> Microsoft IE 11 不支持
