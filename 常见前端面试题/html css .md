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

##什么叫优雅降级和渐进增强？     
**渐进增强 progressive enhancement**：     
针对低版本浏览器进行构建页面，保证最基本的功能，然后再针对高级浏览器进行效果、交互等改进和追加功能达到更好的用户体验。     
**优雅降级 graceful degradation**： 
一开始就构建完整的功能，然后再针对低版本浏览器进行兼容。    
**区别**：    
a. 优雅降级是从复杂的现状开始，并试图减少用户体验的供给    
b. 渐进增强则是从一个非常基础的，能够起作用的版本开始，并不断扩充，以适应未来环境的需要   
c. 降级（功能衰减）意味着往回看；而渐进增强则意味着朝前看，同时保证其根基处于安全地带  

##sessionStorage 、localStorage 和 cookie 之间的区别     
**共同点**：用于浏览器端存储的缓存数据   
**不同点**：      
(1)存储内容是否发送到服务器端：当设置了Cookie后，数据会发送到服务器端，造成一定的宽带浪费；web storage,会将数据保存到本地，不会造成宽带浪费；     
(2)数据存储大小不同：Cookie数据不能超过4K,适用于会话标识；web storage数据存储可以达到5M;     
(3)数据存储的有效期限不同：cookie只在设置了Cookid过期时间之前一直有效，即使关闭窗口或者浏览器；sessionStorage,仅在关闭浏览器之前有效；localStorage,数据存储永久有效；   
(4)作用域不同：cookie和localStorage是在同源同窗口中都是共享的；sessionStorage不在不同的浏览器窗口中共享，即使是同一个页面；   

##Web Storage与Cookie相比存在的优势：   
(1)存储空间更大：IE8下每个独立的存储空间为10M，其他浏览器实现略有不同，但都比Cookie要大很多。    
(2)存储内容不会发送到服务器：当设置了Cookie后，Cookie的内容会随着请求一并发送的服务器，这对于本地存储的数据是一种带宽浪费。而Web Storage中的数据则仅仅是存在本地，不会与服务器发生任何交互。    
(3)更多丰富易用的接口：Web Storage提供了一套更为丰富的接口，如setItem,getItem,removeItem,clear等,使得数据操作更为简便。cookie需要自己封装。   
(4)独立的存储空间：每个域（包括子域）有独立的存储空间，各个存储空间是完全独立的，因此不会造成数据混乱。


