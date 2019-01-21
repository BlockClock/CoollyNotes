#### 版本号
```
git --version

```
#### 用户名/邮箱
```
git config --global user.name "Coolly"
git config --global user.email "zhongxiaohai@gmail.com"
```

#### 创建本地库
```
git init
```

#### 查看暂存区
```
git status
```

#### 添加文件到暂存区
```
git add ...
```

#### 重置暂存区(文件从缓存区移开)
```
git reset
```

#### 提交缓存区内容到存储库
```
git commit -m "Message"
```

#### 查看提交记录
```
git log
```

#### 推送(这边绕过设置key的步骤 账户密码以明文方式显示)
```
git push https://Username:Password@github.com/Username/RepositoryName.git master
```

#### 克隆(这边基本都是克隆开源库 直接使用原地址)
```
git clone https://github.com/Username/RepositoryName.git folder
```

#### 拉取(这边基本都是拉取开源库 直接使用原地址)
```
git pull https://github.com/Username/RepositoryName.git master
```


#### 创建分支
```
git branch branch-name
```

#### 查看所有分支
```
git branch
```

#### 切换分支
```
git checkout branch-name
```

#### 合并分支
```
git checkout main-name
git merge branch-name

```

#### 删除分支
```
git branch -d branch-name
```

#### 合并第一条并行分支
```
git checkout main-name
git merge branch-name-1
```

#### 如果有冲突
```	
git add ...
git commit -m "Message"
```

#### 合并第二条并行分支
```
git branch branch-name-2
git rebase main-name
```

#### 如果有冲突
```	
git add ...
git rebase --continue
```

#### 然后在合并到主干
```
git checkout main-name
git merge branch-name-2
```

这样gitk显示的图表会清晰很多