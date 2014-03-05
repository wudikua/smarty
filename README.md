Smarty2.6支持模版继承
=============
使用
-------------
>将Smarty和Smarty_Compiler覆盖smarty源码的文件

>{block name=xx}
>创建一个block，可以让被继承的模版重写
>{/block}

>{extend file=base.tpl}
>通过extend标签继承

特性
-------------
>1.支持多继承.
>2.支持block的嵌套
>3.block中支持name=xx.after name=xx.before来更改父模版(主要是因为自己没实现类似于super方法，对父模版重用)
>4.支持重写某个block后再创建block嵌套

两点说明
-------------
>1.block标签独占一行
>2.子模版中非block标签内的内容会被忽略
