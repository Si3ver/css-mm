本项目为《CSS实战手册》第四版的读书笔记。

# CSS页面布局

布局类型
+ 固定宽度布局
+ 流式布局
+ 响应式web设计（RWD）

## 基于浮动的布局 -- float

[自己按照书中的例子做了一个](https://si3ver.github.io/css-mm/ch13.html)

说明

+ 三栏流式布局
+ 侧边栏宽度为百分比 20% 60% 20%
+ 把box-sizing设为border-box，使计算简单。
+ 为footer添加clear清除浮动 -> 使用伪类更好
+ trick, 顶部横幅横向布满屏幕，页眉和页脚的文字与内容均居中

```css
nav ul, header h1, footer p, .contentWrapper {
	max-width: 1200px;
	margin: 0 auto;
}
```

注意事项：

+ 小心宽度不够导致浮动下坠
    + 原则，不为分栏div标签设置边框和内边距，为分栏里的元素设置
    + 设置 box-sizing: border-box;

浮动布局的不足：

+ HTML代码顺序，浮动元素需要写在前面，会影响SEO -> 浮动主栏
+ 存在各栏高度不等问题 -> 伪造分栏（为浮动分栏外层添加与分栏宽度一致的背景图or线性渐变）

## 基于定位的布局 -- position

[自己按照书中的例子做了一个]()

## RWD

[自己按照书中的例子做了一个]()

## CSS栅格系统

[自己按照书中的例子做了一个]()

## Flexbox

[自己按照书中的例子做了一个]()


