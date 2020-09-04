1.获取Http响应  
 &emsp;i. 获取文件流  
 &emsp;ii. 解析Body    
2.解析HTML  
 &emsp;i. 使用有限状态机解析token  
 &emsp;ii. 用token生成element和text节点    
&emsp;iii. 组合成DOM结构  
3.解析CSS  
&emsp;i. 收集CSS规则  
&emsp;ii. 判断元素跟CSS规则是否匹配  
&emsp;iii. 计算CSS规则优先级  
&emsp;iv. 把优先级更高的CSS规则应用到元素  
4.布局  
&emsp;i. 初始化布局属性默认值  
&emsp;ii. 子元素分行  
&emsp;iii. 计算主轴  
&emsp;&emsp;flexible item的mainSize会根据flex line的剩余尺寸来决定的，剩余尺寸按比均摊  
&emsp;&emsp;当flow-wrap值为nowrap且非flexible item的总尺寸大于flex line尺寸，元素尺寸会被等比压缩  
&emsp;iv. 计算交差轴  
&emsp;&emsp; 当flex-wrap的值为nowrap，把行crossSize设置为容器的crossSize
&emsp;&emsp; 当item的crossSize没有设置时，如果align-items的值为stretch，则把item的crossSize设置为行crossSize，否则为0  
5.绘制  
&emsp;&emsp;i. 根据布局信息绘制整个页面  
CSS  
&emsp;&emsp;At-rules  
&emsp;&emsp;@charset  
&emsp;&emsp;@import  
&emsp;&emsp;@media  
&emsp;&emsp;@page  
&emsp;&emsp;@counter-style  
&emsp;&emsp;@document  
&emsp;&emsp;@keyframes  
&emsp;&emsp;@fontface  
&emsp;&emsp;@supports  
&emsp;&emsp;@namespace  
&emsp;&emsp;@viewport  
rule   
&emsp;Selector  
&emsp;&emsp;selectors_group  
&emsp;&emsp;combinator  
&emsp;&emsp;&emsp;\s  
&emsp;&emsp;&emsp;>  
&emsp;&emsp;&emsp;+  
&emsp;&emsp;&emsp;~  
&emsp;&emsp;simple_selector  
&emsp;&emsp;&emsp;type  
&emsp;&emsp;&emsp;*  
&emsp;&emsp;&emsp;#  
&emsp;&emsp;&emsp;.  
&emsp;&emsp;&emsp;[]  
&emsp;&emsp;&emsp;: and ::  
&emsp;&emsp;&emsp;:not  
&emsp;Declaration  
&emsp;&emsp;Key  
&emsp;&emsp;&emsp;Property  
&emsp;&emsp;&emsp;Variables  
&emsp;&emsp;Value  
