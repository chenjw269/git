  
  
- [远程库](#远程库)
  - [团队内协作](#团队内协作)
  - [团队间协作](#团队间协作)
- [Git 远程库命令](#git-远程库命令)
  - [添加远程库](#添加远程库)
  - [代码推送 push](#代码推送-push)
  - [代码拉取 pull](#代码拉取-pull)
  - [代码克隆 clone](#代码克隆-clone)
  - [添加权限](#添加权限)
  - [跨团队](#跨团队)
  - [SSH 免密登录](#ssh-免密登录)
- [Idea 使用 Github](#idea-使用-github)
  
[返回目录](Readme.md)

##  远程库
  
###  团队内协作
  
  
- 作者 1 （创作）`push`：本地库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 远程库
- 作者 2 （克隆）`clone`：远程库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 本地库
- 作者 2 （修改） `push`：本地库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 远程库
- 作者 1 （采纳） `pull`： 远程库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 本地库
  
###  团队间协作
  
  
- 团队 2 （接收） `fork`：远程库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 远程库
- 团队 2 （克隆） `clone`：远程库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 本地库
- 团队 2 （修改） `push`：本地库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 远程库
- 团队 2 （请求接收） `pull request`
- 团队 1 （同意接收） `merge`：远程库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 远程库
- 团队 1 （采纳） `pull`：远程库 <img src="https://latex.codecogs.com/gif.latex?&#x5C;to"/> 本地库
  
##  Git 远程库命令
  
  
|命令|作用|
|--|--|
|`git remote -v`|查看所有远程库|
|`git remote add xxx xxxx`|添加远程库|
|`git push xxx xxxx`|代码推送|
|`git pull xxx xxxx`|代码拉取|
|`git clone xxxx`|代码克隆|
  
###  添加远程库
  
  
    git remote add xxx xxxx
  
添加远程库，并设置别名
添加之后会出现两个远程库条目，一为拉取，一为上传
  
###  代码推送 push
  
  
    git push xxx xxxx
  
用本地库更新远程库
推送的最小单位是分支
可以通过远程库的别名、或者远程库的地址推送
  
###  代码拉取 pull
  
  
    git pull xxx xxxx
  
用远程库更新本地库
拉取的最小单位是分支
可以通过远程库的别名、或者远程库的地址推送
  
拉取操作会自动更新版本，不需要再添加和提交
  
###  代码克隆 clone
  
  
    git clone xxxx
  
从公共库克隆代码不需要账户
需要先取得远程库的 git 地址
  
`clone` 完成的工作
- 拉取代码
- 初始化本地库
- 创建别名 `origin`
  
###  添加权限
  
  
    Settings → Manage access → Invite a collaborator
  
只有成为项目成员，才能够向远程库推送代码
  
###  跨团队
  
  
在其他远程库右上角点击 fork，将远程库复制到自己的账户
  
创建 `pull request` ，会自动发送给代码复制来源账户的远程库
  
来源账户可以 `merge pull request` 来更新远程库
  
###  SSH 免密登录
  
##  Idea 使用 Github
  
  