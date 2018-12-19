##什么是盒子模型？   
 在网页中，一个元素占有空间的大小由几个部分构成，其中包括元素的内容（content），元素的内边距（padding），元素的边框（border），元素的外边距（margin）四个部分。这四个部分占有的空间中，有的部分可以显示相应的内容，而有的部分只用来分隔相邻的区域或区域。4个部分一起构成了css中元素的盒模型。  
**w3c的盒子模型**： padding和border不被包含在定义的width和height之内。对象的实际宽度等于设置的width值和border、padding之和，即 ( Element width = width + border + padding ) 此属性表现为标准模式下的盒模型。   
**IE的盒子模型**： padding和border被包含在定义的width和height之内。对象的实际宽度就等于设置的width值，即使定义有border和padding也不会改变对象的实际宽度，即 ( Element width = width ) 。  

##浏览器的内核分别是什么?
**IE**: trident内核  
**Firefox**：gecko内核  
**Safari**：webkit内核   
**Opera**：以前是presto内核，Opera现已改用Google Chrome的Blink内核    
**Chrome**：Blink(基于webkit，Google与Opera Software共同开发)    

##css选择器有哪些，选择器的权重的优先级     
**选择器类型**     
1、ID　　#id      
2、class　　.class      
3、标签　　p      
4、通用　　*         
5、属性　　[type="text"]         
6、伪类　　：hover         
7、伪元素　　::first-line     
8、子选择器、相邻选择器       
**权重计算规则**      
1. 第一等：代表内联样式，如: style=””，权值为1000。      
2. 第二等：代表ID选择器，如：#content，权值为0100。        
3. 第三等：代表类，伪类和属性选择器，如.content，权值为0010。      
4. 第四等：代表类型选择器和伪元素选择器，如div p，权值为0001。         
5. 通配符、子选择器、相邻选择器等的。如*、>、+,权值为0000。        
6. 继承的样式没有权值。     

##px和em的区别         
相同点：px和em都是长度单位；          
异同点：px的值是固定的，指定是多少就是多少，计算比较容易。em得值不是固定的，并且em会继承父级元素的字体大小。浏览器的默认字体高都是16px。所以未经调整的浏览器都符合:1em=16px。那么12px=0.75em, 10px=0.625em。  

##position的值， relative和absolute分别是相对于谁进行定位的          
**absolute** :生成绝对定位的元素，不为元素预留空间，通过指定元素相对于最近的非 static 定位祖先元素的偏移，来确定元素位置。绝对定位的元素可以设置外边距（margins），且不会与其他边距合并。           
**fixed** （老IE不支持）生成绝对定位的元素，不为元素预留空间，而是通过指定元素相对于屏幕视口（viewport）的位置来指定元素位置。元素的位置在屏幕滚动时不会改变。打印时，元素会出现在的每页的固定位置。fixed 属性会创建新的层叠上下文。当元素祖先的 transform 属性非 none 时，容器由视口改为该祖先。    
**relative** 生成相对定位的元素，元素先放置在未添加定位时的位置，再在不改变页面布局的前提下调整元素位置（因此会在此元素未添加定位时所在位置留下空白）。             
**static** 默认定位属性值。该关键字指定元素使用正常的布局行为，即元素在文档常规流中当前的布局位置。此时 top, right, bottom, left 和 z-index 属性无效。           
**sticky** 盒位置根据正常流计算(这称为正常流动中的位置)，然后相对于该元素在流中的 flow root（BFC）和 containing block（最近的块级祖先元素）定位。在所有情况下（即便被定位元素为 table 时），该元素定位均不对后续元素造成影响。当元素 B 被粘性定位时，后续元素的位置仍按照 B 未定位时的位置来确定。position: sticky 对 table 元素的效果与 position: relative 相同。           

[CSS实现垂直居中的5种方法](https://www.qianduan.net/css-to-achieve-the-vertical-center-of-the-five-kinds-of-methods/)      

[常用的清除浮动方法](https://www.cnblogs.com/nxl0908/p/7245460.html)    


