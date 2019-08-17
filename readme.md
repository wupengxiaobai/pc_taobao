# 淘宝首页 PC

## html 知识点

- head (头部信息)

  - ico 网站图标
    规则：1. 根目录 2. ico 后缀格式图片
  - base 默认链接
    a 标签的默认路径和打开方式

- 三栏布局(中间居中)

- table 实现九宫格
  ```CSS
    /*reset.css*/
    table {
        border-collapse: collapse; /*边框模式，合并模式*/
    }
    td, th{
        padding: 0;
    }
    /*index.css*/
    table{
        width:290px;
        height:320px;
        /*行列算法，根据tab宽高自动计算 td 宽高保持一致*/
        table-layout: fixed;
    }
  ```

## css 知识点

- @规则
  ```
  @charset    设置样式编码
  @import     导入其它样式
  @media      媒体查询
  @font-face  自定义字体
  ```
- 行高 `line-height`

  ```css
  body {
    font: 12px/1.5 tahoma, arial, "Hiragino Sans GB", "\5b8b\4f53", sans-serif;
    /* 
          line-height: normal;
          line-height: 2em;
          line-height: 150%;
          line-height: 1.5;
          line-height: 30px;
      */
    /* 
          line-height 
          除px设置固定外，其它都是根据元素字体大小进行相对地设置行高    
          多种相对行高表现中唯 1.5 能以固定倍率的方式继承给后代元素，其余则都是根据父级行高进行设置。 
      */
    /*
          字体中的 unicode 编码，以让不同语言中可以正常识别中文汉字。
      */
  }
  ```

- calc(100% - 190px) IE9+

- css hack

  ```CSS
  /*IE支持rgba兼容写法, 仅ie下有效*/
  .firstLeft {
    background: rgba(0, 0, 0, .3);

    /*仅IE9及以下浏览器认识*/
    background: #0000\9;
    filter: alpha(apacity=30);
  }
  ```

- css 背景渐变兼容

  ```CSS
  .bg{
    background-image: linear-gradient(135deg, #ff971b, #ff5000);
    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffff971b', endColorstr='#ffff5000', GradientType=1);
  }
  ```

- 空格换行属性

  ```CSS
    .text{
      /*我的 他们*/
      word-break: keep-all
    }
  ```

- 图片垂直居中

  - display: table-cell;

- 雪碧图使用

  - background-position

- webp 格式图片
  相比 jpg 等格式图片小很多，且没有其他副作用。 不兼容 ie

## 三方依赖

- iconfont
  - 字体图标的使用
