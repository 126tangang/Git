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

![image-20210904155012662](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904155012662.png)

### 2.初始化本地库

```
git init
```

![image-20210905084220989](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904155012662.png)

初始化之后会出现.git文件

![image-20210904155447094](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904155447094.7hha3kns6dc0.png)

该文件正常情况下被隐藏，需手动打开

![image-20210904155628651](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904155628651.6hti8vj41ao0.png)

### 3.查看本地库状态

```
git status
```

#### 首次查看：

![image-20210904160333797](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904160333797.emp77y4olzs.png)

#### 修改文件：

![image-20210904160446048](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904160446048.5w37klei9to0.png)

#### 修改文件时的命令：

|        i(insert)        |  修改文件  |
| :---------------------: | :--------: |
|           Esc           |  退出修改  |
| yy(以下都需要ESC后输入) | 复制当前行 |
|            p            |    粘贴    |
|          ：wq           |    保存    |

![image-20210904164026758](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904164026758.tketvm0ai6o.png)

#### 修改后查看：

![image-20210904162012650](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904162012650.2xdqhfo6lem0.png)

### 4.添加暂存区

```
git add 文件名
```

添加到暂存区后查看状态：

![image-20210904161831712](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904161831712.15sn7a26l2ak.png)	

### 5.提交到本地库

```
git commit -m "日志信息" 文件名
```

![image-20210904162401859](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904162401859.36qdtsu78sa0.png)

提交到本地库后查看状态：

![image-20210904162526904](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904162526904.5061bvkti5k0.png)

### 6.查看历史版本

#### 查看版本信息：

```
git reflog
```

![image-20210904162814051](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904162814051.29icb179qakg.png)

#### 查看版本详细信息

```
git log	
```

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904163254429.2n6nts3o07s0.png" alt="image-20210904163254429" style="zoom: 50%;" />

### 7.版本穿梭

```
git reset --hard 版本号
```

查看版本信息，当前版本是**52a5ba8**

![image-20210904163635896](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904163635896.2k1iymyz1oo0.png)

切换到第一次提交的版本：

![image-20210904164250934](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904164250934.ujnu0wntuz4.png)

此时再次查看版本信息，指针指向91c8989，也就是第一个版本

![image-20210904164406437](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904164406437.2955bdp7mrpc.png)

查看第一个版本文件信息

![image-20210904164444175](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904164444175.276qup1n67ok.png)

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

![image-20210904165227999](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904165227999.5jbdsxkp18w0.png)

### 创建分支

```
git branch 分支名
```

创建名为test的分支，刚创建的test分支将主分支master上的内容复制了一份

![image-20210904165549861](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904165549861.5tbd8ppltjw0.png)

### 切换分支

```
git checkout 分支名
```

![image-20210904170335830](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904170335830.37zrxplorqm0.png)

查看hot-fix分支下文件内容

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904170447954.j1tfxgme55c.png" alt="image-20210904170447954" style="zoom:50%;" />

### 合并分支

```
git merge 分支名
```

<img src="https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904171024354.4piipglkx120.png" alt="image-20210904171024354" style="zoom:50%;" />

### 产生冲突与解决冲突

test分支下hello.txt文件

![image-20210904171400295](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904171400295.266480myv04g.png)

master主分支下hello.txt文件

![image-20210904172333206](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904172333206.6sjaeb1v3mg0.png)

手动合并冲突代码

![image-20210904173413450](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904173413450.51ue8ep9xsk0.png)

合并文件后添加到本地库是不能加文件名

![image-20210904173823476](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904173823476.29jx0s6qzxus.png)

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

![image-20210904175043347](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904175043347.gtv54yir2ew.png)

### 创建远程仓库别名

```
git remote add 别名 远程地址
```

![image-20210904182412374](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904182412374.6c2xggl4bqc0.png)

### 推送本地分支到远程仓库

```
git push 别名 分支名
```

![image-20210904185417987](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904185417987.1jyal9srf3y8.png)

![image-20210904190040836](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904190040836.38sbwf7l7lw0.png)

### 克隆远程仓库到本地

```
git clone 远程地址
```

![image-20210904190939302](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904190939302.6fm1o4pm1bc0.png)

成功克隆到桌面上

![image-20210904191120525](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904191120525.30i2zpb5uw60.png)

### 拉取远程库内容

```
git pull 远程库地址别名 远程分支名
```

先在GitHub上改变hello.txt文件，此时本地分支上没有最后一行3

![image-20210904191520980](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904191520980.5hgq1eidj9k0.png)

将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并

![image-20210904192451561](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904192451561.456xjzt6b520.png)

hello.txt已经更新

![image-20210904192620465](https://raw.githubusercontent.com/126tangang/image-hosting/master/typora-git-images/image-20210904192620465.9mlxpxzawjc.png)

