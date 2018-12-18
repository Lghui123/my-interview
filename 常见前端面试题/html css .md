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




