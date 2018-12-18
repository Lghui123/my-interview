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



