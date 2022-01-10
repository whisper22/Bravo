### 序章

仓库管理同步教程：

[如何将本地的代码同步到GitHub或者将GitHub更改后的代码同步到本地 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/405996335)

https://blog.csdn.net/chenzhijie101/article/details/79512336

菜鸟教程需要过一遍：

https://www.runoob.com/git/git-tutorial.html

以下简明教程写的不错：

https://www.runoob.com/manual/git-guide/

图解git将原理讲的十分清晰：

http://marklodato.github.io/visual-git-guide/index-zh-cn.html

Git完整命令手册地址：

http://git-scm.com/docs

#### 实际操作记录

下载Git。

构建仓库。

建立SSH秘钥。

在本地创建空文件夹。

克隆仓库至本地。

将本地文档的变更上传至Github：

<img src="C:\Users\HY119004\AppData\Roaming\Typora\typora-user-images\image-20220107173759889.png" alt="image-20220107173759889" style="zoom:80%;" />

### 基础操作学习

#### 将代码仓库下载至本地

1. 创建仓库，添加SSH秘钥

2. 进入仓库，选择Code下SSH复制按钮

3. 本地新建空文件夹用于存储仓库

4. 该文件目录下右键选择“Git bash here”

5. 下载仓库，命令如下

```c
pwd	→ 查看当前位置
git clone "/path/to/repository" → 通过SSH链接克隆仓库内容
```

#### 将GitHub上修改内容同步到本地

1. GitHub上修改完之后保存内容
2. 进入本地文件夹，右键“Git bash here”
3. 更新本地仓库，命令如下：

```c
pwd → 查看当前位置
git pull origin → 进行更新
```

#### 将本地修改内容上传至GitHub

1. 本地修改完成后保存
2. 文件夹右键“Git bash here”
3. 更新线上仓库，命令如下：

```c
pwd → 查看当前位置
git add. → 添加当前目录下的所有文件到暂存区
git commit -m 'update' → 提交暂存区（更新的文件）？
git push → 将本地分支版本推送到远程并合并
```

