### position的几种属性
    absolute: 生成绝对定位，相对于static定位以外的第一个父元素进行定位
    fixed：生成绝对定位，相对浏览器窗口进行定位
    relative： 生成相对定位，相对于其正常位置进行定位
    static： 默认值，没有定位
    inherit： 从父元素继承position属性的值
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