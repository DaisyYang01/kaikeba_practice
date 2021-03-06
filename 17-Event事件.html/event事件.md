# 第十七章 Event事件



## 课前准备

- 工具
  - 编辑器 VSCode
  - 浏览器 Chorme
- 前置知识
  - DOM
  - BOM
  - ES6

## 课堂主题

1. 讲解js中各种事件的使用及实战

## 课堂目标

1. 掌握js当中的常用事件

## 知识点

- 默认事件：浏览器给的功能

- 事件监听器
  - 事件监听和事件绑定的区别 
  - addEventListener(type, listener[, options|useCapture])
    - 事件流
      - 事件冒泡
      - 事件捕获
    - 事件监听相关配置(options)
      - capture   是否在捕获阶段执行
      - once   是否只执行一次
      - passive  阻止取消默认事件 （拒绝阻止默认行为）
  - removeEventListener(event, fn) 取消事件监听   （不能用匿名函数）
- Event 事件对象
  - Event.target（事件触发的目标源元素）、Event.currentTarget（事件绑定的元素） 事件源
  - 事件委托(事件代理)
    - 事件委托的优点
      1. 可减少需要添加事件绑定的元素
      2. 可给新增DOM元素添加事件（在不刷新页面的情况下）
    - 事件委托的缺点
      1. 事件处理函数中需要判断事件源增加逻辑复杂度。
      2. 祖父级和事件源之间不能有阻止冒泡 
  - mousenter、mouseleave 事件
  - Event.stopPropagation()、Event.cancelBubble 取消冒泡   
  - Event.clientX、Event.clientY、Event.pageX、Event.pageY 鼠标位置获取
- contextmenu 事件 
  - return false 和 Event.preventDefault() 阻止默认事件   

- 兼容
  - event || window.event

- 键盘事件
  - keydown、keyup
  - Event.keyCode、Event.key
  - Event.altKey、Event.ctrlKey、Event.shiftKey
  - 制作组合键 
- 拖拽思路详解
  - mousedown、mousemove、mouseup
    - mousedown 点鼠标左键、右键、中键都可以触发
    - e.button: 0 左键，1 中键，2 右键
  - 拖拽公式：元素当前位置 = (鼠标当前位置 - 鼠标初始位置) + 元素初始位置
  - 拖拽问题修复
  - 限制范围拖拽
- 鼠标滚动事件
  - mousewheel 和 DOMMouseScroll 事件
  - Event.wheelDelta 和  Event.detail 滚轮方向获取
- 其他常用事件：
  - dblclick
  - selectstart 选中文字事件（浏览器默认 ctrl+A 也会触发选中事件）
  - blur、focus、change、input、submit、reset
  - 表单其他方法：blur()、focus()、select()


### 自定义事件

## 课堂案例

- 案例：下拉菜单（取消事件冒泡）
- 案例：留言板（事件委托/代理）
- 案例：自定义右键菜单
- 案例：放大镜
- 案例：键盘操作元素位置
- 案例：拖拽实现
- 案例：鼠标滚轮事件兼容
- 

## 总结



## 作业 && 答疑



## 下节课预告


## 案例
- 下拉菜单
- 右键菜单
- 留言板




