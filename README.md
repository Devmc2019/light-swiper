# light-swiper

## 使用

### 方式一

```html

<div class="light-swiper" style="width: 480px; height: 270px;">
    <img src="./images/1.jpg" data-href="https://www.baidu.com" alt="">
    <img src="./images/2.jpg" alt="">
    <img src="./images/3.jpg" alt="">
</div>
```

```javascript
new LightSwiper('.light-swiper', {
    draggable: false,
    target: '_blank'
});    
```

### 方式二

```html

<div class="light-swiper-2" style="width: 480px; height: 270px; margin-top: 4rem"></div>
```

```javascript
new LightSwiper('.light-swiper-2', {
    images: [
        {
            url: './images/1.jpg',
            href: 'https://www.baidu.com'
        },
        {
            url: './images/2.jpg'
        },
        './images/3.jpg'
    ],
    autoplay: false,
    showDots: 'hover',
    showButtons: 'hover',
    target: '_blank'
});
```

## 配置

```json5
{
  // 图片  [url] or [{url,href}]
  images: [],
  // 图片切换间隔
  interval: 5000,
  // 是否自动播放
  autoplay: true,
  // 动画播放时间
  duration: 1000,
  // 链接打开位置  _self,_blank,_parent,_top
  target: '_self',
  // 图片是否可拖动
  draggable: false,
  // 左边按钮的图片
  leftButtonImage: '',
  // 右边按钮的图片
  rightButtonImage: '',
  // 当鼠标悬浮在左右按钮、小圆点上时，停止自动播放
  stopOnMouseover: true,
  // 切换箭头的显示时机  always,hover,never
  showButtons: 'always',
  // 切换圆点的显示时机  always,hover,never
  showDots: 'always'
}
```
