### component.js中的Component的构造器

1. properties : 向组件传值
2. data : 组件默认的数据
3. methods : 组件内调用方法，只能在这里写
4. observe : 监听属性和数据变化，监听某个值则以该值名为key

<font color=red>注：参数只有newValue，与properties中的observe不同</font>

5. pageLifetimes : 监听页面生命周期

[![toNQaj.png](https://s1.ax1x.com/2020/06/10/toNQaj.png)](https://imgchr.com/i/toNQaj)

6. lifetimes : 组件生命周期

[![toNGR0.png](https://s1.ax1x.com/2020/06/10/toNGR0.png)](https://imgchr.com/i/toNGR0)

7. behaviors : 组件间代码复用机制，每个 `behavior` 可以包含一组属性、数据、生命周期函数和方法。**组件引用它时，它的属性、数据和方法会被合并到组件中，生命周期函数也会在对应时机被调用，实际与component类似**

   使用方法：

   1. 创建behavior.js文件（自定义命名）

   2. 注册 Behavior组件 ( 如Componet内使用Componet({})注册，而Behavior中则是  Behavior({}) 进行注册 )

   3. 注册过后，通过expert导出

   4. 在相应组件中通过import引入，并且在Component中引用

      [![NeviwV.png](https://s1.ax1x.com/2020/06/18/NeviwV.png)](https://imgchr.com/i/NeviwV)

