## AppKit 的事件处理

> 在*AppKit*中的事件都处于一个响应的链条中,这个链条是由一个叫做**`NSResponder`**的类定义的,这个响应链条其实是一个列表,它里面装满了能够响应用户事件的对象.当用户点击鼠标,或者按下键盘的某个键,或者触摸触控板,都会生成一个`Event`事件,然后在响应链条中寻找可以处理这个事件的对象对事件进行处理.
> 一个对象如果可以处理事件,那么这个对象必须继承自**`NSResponder`**这个类.在AppKit中,*NSApplication*,*NSWindow*,*NSView*都继承自**`NSResponder`**
