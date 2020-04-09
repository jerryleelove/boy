#### 1.1 流程

1. 工作区

1. 暂存区
2. Git仓库

#### 1.2本地仓库

##### 1. 全局配置

- ```shell
  git config --global user.name "用户名"
  ```

- ```shell
  git config --global user.email "邮箱地址"
  ```

##### 2. 创建仓库

1. 先创建一个文件夹

2. 进入到这个目录

3. Git仓库的初始化（让Git知道他要管理这个仓库）

   ```shell
   git init
   ```

##### 3. Git常用指令操作

- 查看当前状态

  ```shell
  git status
  ```

- 添加到缓存区

  ```shell
  git add 文件1
  git add 文件1 文件2 文件3
  git add . 
  ```

- 提交到本地仓库

  ```shell
  git commit -m "注释内容"
  ```

#### 1.3 版本回退

1. 常看版本，确定需要回到的时刻

   ```shell
   git log
   git log --pretty=oneline
   ```

2. 回退操作

   ```shell
   git reset --hard 版本号
   ```

   > 当回退到过去后想再回来需要查看历史操作

   ```shell
   git reflog
   ```

#### 2.2 两种常规使用方法

##### 2.2.1 基于http协议

1. 创建空目录

2. 克隆

   ```shell
   git clone url
   ```

3. 提交到线上仓库

   ```shell
   git push
   ```

   > 首次提交，需要配置权限
   >
   > 在.git/config中的url前边添加“用户名”:“密码”@

4. 拉取线上仓库

   ```shell
   git pull
   ```

##### 2.2.2 基于ssh协议

1. 安装openssh

2. 设置密钥

   ```shell
   ssh-keygen -t rsa -C "邮箱"
   ```
   
   > 问题的解决办法
   >
   > 1. <img src="/solution1.jpg"  />2.![](/solution2.jpg)

#### 其他

过滤

