### Doctype作用? 严格模式与混杂模式如何区分？它们有何意义?
    告诉浏览器以何种模式来渲染文档 
    1. 严格模式的排版和JS运作模式是，以浏览器支持的最高标准运行
    2. 混杂模式中，页面以宽松的向后兼容的方式呈现，模拟老式浏览器的行为以防止站点无法工作
    DOCTYPE不存在或格式不正确会导致文档以混杂模式呈现
### 行内元素,块状元素,行内块状元素分别有哪些，区别？
    行内元素：span b i  
            设置宽高无效，对margin仅设置左右方向有效 上下无效，padding设置上下左右都有效，不会自动换行
    块状元素：div p ul ol li dl dt dd
              可以设置宽高，margin,padding都有效，自动换行，默认从上到下排列
    行内块状元素：不自动换行，可设置宽高，margin,padding都有效，从左到右排列
    转换方式  display:inline   display:inline-block   display:block
    