### position的几种属性
    absolute: 生成绝对定位，相对于static定位以外的第一个父元素进行定位
    fixed：生成绝对定位，相对浏览器窗口进行定位
    relative： 生成相对定位，相对于其正常位置进行定位
    static： 默认值，没有定位
    inherit： 从父元素继承position属性的值
### 标准盒模型和IE盒模型
    盒模型：内容(content)、填充(padding)、边界(margin)、 边框(border)
    区别：IE的content部分包括border padding 
    转换：转IE盒模型 - box-sizing:border-box；转标准盒模型 - box-sizing:content-box
### css选择器
    1. id选择器(#id)
    2. 类选择器(.class)
    3. 标签选择器(div,span)
    4. 相邻选择器(img+p) 同一个父元素，相邻紧跟的第一个p元素
    5. 兄弟选择符(p~span) 同一个父元素，位置无须紧邻，只须同层级，A~B 选择A元素之后所有同层级B元素
    6. 子选择器(div>span)
    7. 后代选择器(div span)
    8. 伪类选择器(a:hover,a:first-child,a:nth-child) 
    9. 伪元素选择器(p::after)
### css属性继承
    可继承样式：font-size,font-famlily,color
    不可继承样式：border padding margin width height
### css 优先级 
    @important>内联>id>class>tag>通配符>继承>浏览器默认属性
    
### 水平垂直居中
      <body>
        <div></div>
      </body>
    1. div {
          width: 300px;
          height: 300px;
          background: green;
          position: absolute;
          top: 0;
          left: 0;
          right: 0;
          bottom: 0;
          margin: auto;
        }
    2. div {
          width: 300px;
          height: 300px;
          background: green;
          position: absolute;
          top: 50%;
          left: 50%;
          margin-left: -150px;
          margin-top: -150px;
        }
    3. div {
          width: 300px;
          height: 300px;
          background: green;
          position: absolute;
          top: 50%;
          left: 50%;
          transform: translate(-50%, -50%)
        }
    4.  body {
          display: flex;
          align-items: center;
          justify-content: center;
        }
    5. body {
          width: 100vw;
          height: 100vh;
          display: table-cell;
          text-align: center;
          vertical-align: middle;
        }
        div {
          background: green;
          padding: 20px;
          display: inline-block;
        }
    6. body {
          width: 100vw;
          height: 100vh;
          display: grid;
        }
        div {
          background: green;
          padding: 20px;
          align-self: center;
          justify-self: center;
        }