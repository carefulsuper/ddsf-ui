# Card
卡片组件
### 示例
<m-card imgSrc="/java.jpg" summary="看看如何引入组件"/>

### 代码
```html
<m-card imgSrc="/java.jpg" summary="看看如何引入组件"/>
```

### Attributes
| 参数 | 说明 | 类型 | 是否必要 | 默认值 
| --- | ---- | ----- | ------ | ------ |
| width | 卡片的宽度 | Number | false | - |
| imgSrc | 图片资源地址 | String | true | - |
| imgHeight | 图片的高度 | Number | false | - |
| summary | 卡片的概要 | String/Slot | false | - |
| footer | 卡片底部 | Slot | false | - |