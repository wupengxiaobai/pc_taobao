# 淘宝首页 PC

## html 知识点
- head (头部信息)
    + ico 网站图标
        规则：1. 根目录 2. ico后缀格式图片
    + base 默认链接
        a 标签的默认路径和打开方式

## css 知识点
-   @规则
    ```
    @charset    设置样式编码
    @import     导入其它样式
    @media      媒体查询
    @font-face  自定义字体
    ```
-   行高 `line-height`
    ```css
    body{
        font: 12px/1.5 tahoma, arial, 'Hiragino Sans GB', '\5b8b\4f53', sans-serif;
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

## 三方依赖
-   iconfont
    +   字体图标的使用
    