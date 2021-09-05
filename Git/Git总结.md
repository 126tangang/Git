# Git总结

## Git常用命令



| 命令                                 |        用途        |
| :----------------------------------- | :----------------: |
| git config --global user.name 用户名 |    设置用户签名    |
| git config --global user.email 邮箱  |    设置用户签名    |
| **git initc**                        |  **初始化本地库**  |
| **git status**                       | **查看本地库状态** |
| **git add 文件名**                   |  **添加到暂存区**  |
| **git commit -m "日志信息" 文件名**  |  **提交到本地库**  |
| **git reflog**                       |  **查看历史记录**  |
| **git reset --hard 版本号**          |    **版本穿梭**    |

### 1.设置用户签名

```
git config --global user.name 用户名 
git config --global user.email 邮箱
//查看用户签名
cat ~/.gitconfig
```

查看用户签名：

![image-20210904155012662](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904155012662.png)

### 2.初始化本地库

```
git init
```

![image-20210905084220989](../../../../AppData/Roaming/Typora/typora-user-images/image-20210905084220989.png)

初始化之后会出现.git文件

![image-20210904155447094](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904155447094.png)

该文件正常情况下被隐藏，需手动打开

![image-20210904155628651](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904155628651.png)

### 3.查看本地库状态

```
git status
```

#### 首次查看：

![image-20210904160333797](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904160333797.png)

#### 修改文件：

![image-20210904160446048](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904160446048.png)

#### 修改文件时的命令：

|        i(insert)        |  修改文件  |
| :---------------------: | :--------: |
|           Esc           |  退出修改  |
| yy(以下都需要ESC后输入) | 复制当前行 |
|            p            |    粘贴    |
|          ：wq           |    保存    |

![image-20210904164026758](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904164026758.png)

#### 修改后查看：

![image-20210904162012650](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904162012650.png)

### 4.添加暂存区

```
git add 文件名
```

添加到暂存区后查看状态：

![image-20210904161831712](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904161831712.png)

### 5.提交到本地库

```
git commit -m "日志信息" 文件名
```

![image-20210904162401859](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904162401859.png)

提交到本地库后查看状态：

![image-20210904162526904](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904162526904.png)

### 6.查看历史版本

#### 查看版本信息：

```
git reflog
```

![image-20210904162814051](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904162814051.png)

#### 查看版本详细信息

```
git log	
```

<img src="C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904163254429.png" alt="image-20210904163254429" style="zoom: 67%;" />

### 7.版本穿梭

```
git reset --hard 版本号
```

查看版本信息，当前版本是**52a5ba8**

![image-20210904163635896](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904163635896.png)

切换到第一次提交的版本：

![image-20210904164250934](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904164250934.png)

此时再次查看版本信息，指针指向91c8989，也就是第一个版本

![image-20210904164406437](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904164406437.png)

查看第一个版本文件信息

![image-20210904164444175](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904164444175.png)

## Git分支操作



|        命令         |             作用             |
| :-----------------: | :--------------------------: |
|  git branch 分支名  |           创建分支           |
|    git branch -v    |           查看分支           |
| git checkout 分支名 |           切换分支           |
|  git merge 分支名   | 把指定的分支合并到当前分支上 |

### 查看分支

```
git branch -v 分支名
```

共有两个分支，当前在master分支下，版本是91c8989,日志信息为first commit

![image-20210904165227999](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904165227999.png)

### 创建分支

```
git branch 分支名
```

创建名为test的分支，刚创建的test分支将主分支master上的内容复制了一份

![image-20210904165549861](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904165549861.png)

### 切换分支

```
git checkout 分支名
```

![image-20210904170335830](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904170335830.png)

查看hot-fix分支下文件内容

![image-20210904170447954](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904170447954.png)

### 合并分支

```
git merge 分支名
```

![image-20210904171024354](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904171024354.png)

### 产生冲突与解决冲突

test分支下hello.txt文件

![image-20210904171400295](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904171400295.png)

master主分支下hello.txt文件

![image-20210904172333206](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904172333206.png)

手动合并冲突代码

![image-20210904173413450](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904173413450.png)

合并文件后添加到本地库是不能加文件名

![image-20210904173823476](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904173823476.png)

## GitHub操作

|                命令                 |                           作用                           |
| :---------------------------------: | :------------------------------------------------------: |
|            git remote -v            |                 查看当前所有远程地址别名                 |
|    git remote add 别名 远程地址     |                          起别名                          |
|         git push 别名 分支          |               推送本地分支上的内容到远程库               |
|         git clone 远程地址          |                将远程仓库的地址克隆到本地                |
| git pull 远程库地址别名  远程分支名 | 将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并 |

### 查看远程仓库别名

```
git remote -v
```

![image-20210904175043347](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904175043347.png)

### 创建远程仓库别名

```
git remote add 别名 远程地址
```

![image-20210904182412374](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904182412374.png)

### 推送本地分支到远程仓库

```
git push 别名分支名
```

![image-20210904185417987](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904185417987.png)

![image-20210904190040836](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904190040836.png)

### 克隆远程仓库到本地

```
git clone 远程地址
```

![image-20210904190939302](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904190939302.png)

成功克隆到桌面上

![image-20210904191120525](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904191120525.png)

### 拉取远程库内容

```
git pull 远程库地址别名 远程分支名
```

先在GitHub上改变hello.txt文件，此时本地分支上没有最后一行3

![image-20210904191520980](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904191520980.png)

将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并

![image-20210904192451561](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904192451561.png)

hello.txt已经更新

![image-20210904192620465](C:\Users\86152\AppData\Roaming\Typora\typora-user-images\image-20210904192620465.png)

