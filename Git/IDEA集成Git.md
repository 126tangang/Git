# IDEA集成Git

## 1.配置Git忽略文件

配置git.ignore和.gitconfig文件

## 2.定位Git程序

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904194406528.png" alt="image-20210904194406528" style="zoom:50%;" />

## 3.初始化本地库

第一步

![image-20210904195209494](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904195209494.png)

第二步：直接OK就好

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904195251486.png" alt="image-20210904195251486" style="zoom: 50%;" />

此时就生成可.git文件

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904195516155.png" alt="image-20210904195516155" style="zoom:50%;" />

同时发现IDEA中的文件颜色变红，代表这些文件还存在工作区中

![image-20210904195647991](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904195647991.png)

## 4.添加到暂存区

右键点击你想添加到暂存区的文件

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904195912111.png" alt="image-20210904195912111" style="zoom: 50%;" />

此时发现文件变为绿色

![image-20210904195955086](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904195955086.png)

## 5.提交到本地库

第一步

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904200458642.png" alt="image-20210904200458642" style="zoom: 50%;" />

第二步

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904200708069.png" alt="image-20210904200708069" style="zoom: 50%;" />

提交到本地库后文件颜色又恢复原来的颜色

![image-20210904202056946](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904202056946.png)

此时更改某个文件其颜色会变成浅蓝色，表示这个文件被追踪过，并且你又修改了该文件

![image-20210904202213376](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904202213376.png)

## 6.切换版本

第一步

![image-20210904202836233](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904202836233.png)

右键点击你想切换的版本

![image-20210904203302537](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904203302537.png)

切换后发现黄色的指针指向第一个版本，黄色指针指向当前版本所在的分支

绿色指针指向主分支master

切换版本后代码会自动变化成当前版本代码

![image-20210904203503818](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904203503818.png)

## 7.创建分支

方法一：右键你想提交的文件

![image-20210904204522078](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904204522078.png)

方法二：点击左下角Git，再点击右下角当前版本

![image-20210904204954988](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904204954988.png)

点击New Branch

![image-20210904205059504](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904205059504.png)

输入分支名

![image-20210904205411103](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904205411103.png)

分支创建完成

![image-20210904205735189](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904205735189.png)

## 8.切换分支

![image-20210904210132623](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904210132623.png)

切换到maser分支

![image-20210904210300378](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904210300378.png)

## 9.合并分支



![image-20210904211700659](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904211700659.png)

当出现冲突时

![image-20210904213630528](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904213630528.png)

手动合并

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904213857016.png" alt="image-20210904213857016" style="zoom:50%;" />

合并完成

![image-20210904214453396](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904214453396.png)

## 10.IDEA集成GitHub

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904215517402.png" alt="image-20210904215517402" style="zoom:50%;" />

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904215620591.png" alt="image-20210904215620591" style="zoom:50%;" />

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904220048327.png" alt="image-20210904220048327" style="zoom:50%;" />

## 11.分享项目到GitHub

![image-20210904220733481](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904220733481.png)

![image-20210904221557635](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904221557635.png)

![image-20210904221246120](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904221246120.png)

成功push到GitHub上

![image-20210904221915593](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904221915593.png)

## 12.推送代码到远程库

第一步

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905074544390.png" alt="image-20210905074544390" style="zoom:50%;" />

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905074652044.png" alt="image-20210905074652044" style="zoom:50%;" />

第二步

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905074809542.png" alt="image-20210905074809542" style="zoom:50%;" />

第三步

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905075130419.png" alt="image-20210905075130419" style="zoom:50%;" />

取一个别名，复制链接，点OK

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905075213806.png" alt="image-20210905075213806" style="zoom:50%;" />

切换到新建的ssh链接

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905075326681.png" alt="image-20210905075326681" style="zoom:50%;" />

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905075427570.png" alt="image-20210905075427570" style="zoom:50%;" />

点击Push到远程库，显示Push成功

![image-20210905075858861](../../../AppData/Roaming/Typora/typora-user-images/image-20210905075858861.png)

远程库相应文件也进行了更新

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905080033347.png" alt="image-20210905080033347" style="zoom:50%;" />

## 13.拉取远程库代码到本地

要想Push成功，首先要保证本地库版本比远程库版本高。所以有时我们需要pull远程库代码

pull同样会涉及到冲突的问题自动合并失败后需要手动合并。

首先在GitHub上更新一下代码，现在远程库与本地代码版本不一致

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905080454184.png" alt="image-20210905080454184" style="zoom:50%;" />

第二步

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905082625120.png" alt="image-20210905082625120" style="zoom:50%;" />

通过SSH方式拉取

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905082706942.png" alt="image-20210905082706942" style="zoom:50%;" />

pull成功

![image-20210905082855158](../../../AppData/Roaming/Typora/typora-user-images/image-20210905082855158.png)

## 克隆代码到本地

第一步

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905083139468.png" alt="image-20210905083139468" style="zoom:50%;" />

第二步，选择你想克隆项目的链接

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210905083410064.png" alt="image-20210905083410064" style="zoom:50%;" />

点击clone即可，就不演示了。
