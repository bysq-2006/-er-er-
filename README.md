# 你好
这是一个能够很方便绘制ER图的程序，拥有GUI界面，简单易上手。<br>
你可以直接下载打包好的exe程序<br>
如果exe程序不能用,请下载Python<br>
也可以下载源代码然后自己安装pyqt5来使用<br>
exe下载地址：通过网盘分享的文件：Draw_ER_diagram.exe
链接: https://pan.baidu.com/s/1pXJSrJq_PJTbmrDWz1KM0g?pwd=0514 提取码: 0514
<br>github不允许上传超过25mb的文件，所以只能用百度网盘了。
<br>教程：https://www.bilibili.com/video/BV14hXkYTE96/?spm_id_from=333.337.search-card.all.click


下面是一些方便后期修改整理思路的东西：<br>
第一眼看到这个一er模型，我就感觉有点像无向图，所以我用了两个东西来存储，一个存储点，一个存储边，对应的就是实体和联系。<br>
正常情况也就是前两个界面，存储的时候主键和外键都是字符串，等到绘图的时候会用一个内置函数转换成角标，这个是为了优化（虽然并没有优化多少）<br>
等到绘图界面会新增几个属性，主要就是实体的xy坐标，还有实体属性的xy坐标和联系那些，反正每一个都有xy坐标。<br>
属性xy坐标的存储方式是一个1对1的列表里面存储长度为二的列表，角标为0的是x，角标为1的是y。<br>
