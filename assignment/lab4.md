#lab4实验报告
##1.死锁截图

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-d8c2742cae6db8b3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
##2.死锁产生四大必要条件
###1.互斥。一个实例每次只能被一个进程占有。
###2.占有且等待。一个进程占有了一个或多个实例，但是它所需要的别的实例被别的进程所占有，且该进程不放弃当前所占有的实例。
###3.非抢占式。进程已经获得的实例，在还没有使用完释放之前不能被别的进程占有。
###4.循环等待。若干进程之间形成一种头尾相接的循环等待资源关系。
##3.对实验程序产生死锁的解释
###实验中我们用到的程序里面我们可以从class A和class B中看出当运行A的时候同时运行B的话就会产生死锁，因为运行A的时候，B所需要的实例会被A所占有。同理B也是这样。
##4.实验体会
###这次实验比较简单，主要是让我们理解死锁的产生，这个之前操作系统也有学过，所以较为轻松。但是实验中我犯了一个低级错误，WINDOWS里面批处理文件是.bat，但是linux里面是.sh，尴尬。还有就是要运行Deadlock.sh的时候要给它权限（在终端输入sudo chmod +x Deadlock.sh），不然运行不了，具体操作如下：

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-8f11d0cb4b7d8748.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
