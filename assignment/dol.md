#dol实例分析与编程
##一、实验要求
###1.修改example2，让3个square模块变成2个
###2.修改example1，使其输出3次方数
##二、代码修改
###代码主要只是做了简单修改
####1.修改square.c文件中的i=i*i为i=i*i*i，表示输出立方
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-b9e73c723d83c56d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
####2.修改example2.xml里面的variable value="3"里面的3为2，表示将3个square模块变成两个
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-649f9fb501e4c451.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
##三、实验结果
###1.example1运行截图，我们可以清楚看到里面的数值是立方后的结果。
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-a6b55d7caa007250.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-b7119d63bce0f9e2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
###2.example2运行截图，我们可以观察得到结果是二次方的结果，而且看.dot我们可以看到里面只有square_0和square_1，表示只有两个模块。
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-b37be04e2e605a7c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-a45b6ff5bb0314ca.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
##四、心得体会
###这次的实验还是比较简单的，应该主要是让我们感受一下dol的工作过程吧。但是有一点就是因为编译运行代码的时候因为使用了sudo语句，所以example1跟example2是需要root权限的，就是我不可以打开或者是删除。但是我们要使得可以得到修改后的效果，就要删除之前的example，所以就需要我们有权限对其进行修改。经过TA的指导，我找到了两种方法删除root权限的文件。
###1.命令行删除。输入sudo rm -rf example1即可。
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-43ccd283d229e459.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
###2.将root权限修改为用户。输入sudo chown -R yan main即可，这样还可以打开文件夹里面的内容了。
![Paste_Image.png](http://upload-images.jianshu.io/upload_images/3229070-661e2ffeac7f1511.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
