# IDEA集成Git

## 1.配置Git忽略文件

配置git.ignore和.gitconfig文件

## 2.定位Git程序

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904194406528.7fnb5b5i19g0.png" style="zoom:50%;" />

## 3.初始化本地库

第一步

![image-20210904195209494](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904195209494.3q0y65h32260.png)

第二步：直接OK就好

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904195251486.58p8t1pi0lw0.png" style="zoom: 50%;" />

此时就生成可.git文件

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904195516155.6zuaavnno100.png" style="zoom:50%;" />

同时发现IDEA中的文件颜色变红，代表这些文件还存在工作区中

![image-20210904195647991](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904195647991.3n9eh3lbkdq0.png)

## 4.添加到暂存区

右键点击你想添加到暂存区的文件

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904195912111.soesu81szqo.png" alt="image-20210904195912111" style="zoom: 50%;" />

此时发现文件变为绿色

![image-20210904195955086](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904195955086.2v40dob78qw0.png)

## 5.提交到本地库

第一步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904200458642.7ifjnmlabhc0.png" style="zoom: 50%;" />

第二步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904200708069.rr4ovnquxbk.png" style="zoom: 50%;" />

提交到本地库后文件颜色又恢复原来的颜色

![image-20210904202056946](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904202056946.1fv6swjr4ov4.png)

此时更改某个文件其颜色会变成浅蓝色，表示这个文件被追踪过，并且你又修改了该文件

![image-20210904202213376](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904202213376.5tc95752o5w0.png)

## 6.切换版本

第一步

![image-20210904202836233](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904202836233.md962j7n5kw.png)

右键点击你想切换的版本

![image-20210904203302537](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904203302537.w4vb226su68.png)

切换后发现黄色的指针指向第一个版本，黄色指针指向当前版本所在的分支

绿色指针指向主分支master

切换版本后代码会自动变化成当前版本代码

![image-20210904203503818](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904203503818.6osvvjmc5400.png)

## 7.创建分支

方法一：右键你想提交的文件

![image-20210904204522078](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904204522078.3toat0ventm0.png)

方法二：点击左下角Git，再点击右下角当前版本

![image-20210904204954988](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904204954988.4uufc2zsnoo0.png)

点击New Branch

![image-20210904205059504](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904205059504.6fmcayirwao0.png)

输入分支名

![image-20210904205411103](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904205411103.3knrglwkoik0.png)

分支创建完成

![image-20210904205735189](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904205735189.4ubbnvaq06q0.png)

## 8.切换分支

![image-20210904210132623](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904210132623.1hwqp369le8w.png)

切换到maser分支

![image-20210904210300378](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904210300378.6l58lueve8k0.png)

## 9.合并分支



![image-20210904211700659](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904211700659.5yiqtb0uik00.png)

当出现冲突时

![image-20210904213630528](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904213630528.3z6sxh0mzfu0.png)

手动合并

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904213857016.2ie5i77q2wi0.png" style="zoom:50%;" />

合并完成

![image-20210904214453396](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904214453396.5pygcflavd00.png)

## 10.IDEA集成GitHub

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904215517402.2hlawnsoggs0.png" style="zoom:50%;" />

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904215620591.5kz8zf0l2c80.png" style="zoom:50%;" />

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904220048327.3d3wj70a1jc0.png" style="zoom:50%;" />

## 11.分享项目到GitHub

![image-20210904220733481](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904220733481.46qgro1imxy0.png)

![image-20210904221557635](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904221557635.4rlg86c5opi0.png)

![image-20210904221246120](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904221246120.1nr26npj9bc0.png)

成功push到GitHub上

![image-20210904221915593](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904221915593.3vjju7k1vts0.png)

## 12.推送代码到远程库

第一步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905074544390.3y6yno3pifk0.png" alt="image-20210905074544390" style="zoom:50%;" />

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905074652044.6oi91qgxmng0.png" style="zoom:50%;" />

第二步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905074809542.1n449ohi7ecg.png" style="zoom:50%;" />

第三步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905075130419.5vjm6c0wfjs0.png" style="zoom:50%;" />

取一个别名，复制链接，点OK

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905075213806.5xsngttw5bk0.png" style="zoom:50%;" />

切换到新建的ssh链接

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905075326681.15zjbxmeqgw0.png" style="zoom:50%;" />

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905075427570.35rbwvf1bly0.png" style="zoom:50%;" />

点击Push到远程库，显示Push成功

![image-20210905075858861](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905075858861.1s81ry0mypxc.png)

远程库相应文件也进行了更新

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905080033347.1864070h9xq8.png" style="zoom:50%;" />

## 13.拉取远程库代码到本地

要想Push成功，首先要保证本地库版本比远程库版本高。所以有时我们需要pull远程库代码

pull同样会涉及到冲突的问题自动合并失败后需要手动合并。

首先在GitHub上更新一下代码，现在远程库与本地代码版本不一致

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905080033347.1864070h9xq8.png" style="zoom:50%;" />

第二步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905082625120.1367twvqq6fk.png" style="zoom:50%;" />

通过SSH方式拉取

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905082706942.465sdpczfeo0.png" alt="image-20210905082706942" style="zoom:50%;" />

pull成功

![image-20210905082855158](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905082855158.1pfbjkw9tbmo.png)

## 克隆代码到本地

第一步

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905083139468.tr7ex8j14uo.png" alt="image-20210905083139468" style="zoom:50%;" />

第二步，选择你想克隆项目的链接

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210905083410064.1mdmqrjo4a1s.png" style="zoom:50%;" />

点击clone即可，就不演示了。
