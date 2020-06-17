## WXS基本与JS一致

### 1.在wxml中使用

[![toYq9P.png](https://s1.ax1x.com/2020/06/10/toYq9P.png)](https://imgchr.com/i/toYq9P)



<font color=red>注意： </font>

1. 需要给每个wxs写一个module=“name”名字
2. 需要通过module.exports = {} 导出数据
3. 需要通过name.data的方式取出数据



### 2.外链模式

1. 建立wxs文件夹

2. 创建相应wxs文件，写相应wxs代码，通过module.export导出

3. 在wxml中使用

   <wxs src="相对路径" module="name" />



