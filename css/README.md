### position的几种属性
    absolute: 生成绝对定位，相对于static定位以外的第一个父元素进行定位
    fixed：生成绝对定位，相对浏览器窗口进行定位
    relative： 生成相对定位，相对于其正常位置进行定位
    static： 默认值，没有定位
    inherit： 从父元素继承position属性的值
### 水平垂直居中
    ```css
     div {
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
    ```
