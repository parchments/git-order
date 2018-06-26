<h1>本地与远程关联 </h1>

<h2>一、设置淘宝镜像（下载速度快）</h2>
<p>       1、下载安装node.js</p>
<p>https://nodejs.org/en/</p>

<p>2、安装cnpm</p>
<p>       npm install -g cnpm --registry=https://registry.npm.taobao.org</p>

<p>3、检查是否设置成功 cnpm -v，出现版本号则成功</p>


<p>二、SSH配置（与远程关联的配置）</p>
<p>       SSH配置：ssh-Keygen</p>
<p>       配置完之后能得知ssh的文件位置，并且复制ssh里面的key??</p>
<p>       然后把复制的key粘贴在github-我的-setting-SSH and GPG keys-Add new中去</p>

<h2>三、本地环境配置：</h2>
<p>       git config --global user.name 'xxx'</p>
<p>       git config --global user.email 123456789@qq.com</p>

四、指令
<p>1、初始化本地仓库：git init</p>
<p>2、添加源仓库：git remote add origin yourgithub（切换到user-ssh地址）</p>
<p>3、把远程仓库的内容下载下来：git pull origin </p>
<p>4、检查绑定情况，查看远程仓库：git remote -v</p>
<p>5、查看当前文件的状态： git status</p>
<p>6、提交到暂存区： git add (如果单个文件就像index.html，如果多个文件就用“ . ”点的方式)</p>
<p>       暂存区用处：有修改但是没写完就不能提交到本地仓库，提交到本地仓库都叫一个版本，万一有bug提交后有人合并就会出问题。暂存区会被最新的代码覆盖之前的代码</p>
<p>       放到暂存区：</p>
<p>7、提交到本地仓库：git commit -m ' 提交信息的简介 '</p>
<p>8、提交内容到远程仓库： git push</p>
<p>9、撤销：git checkout -- index.html</p>
<p>10、版本号回退：</p>
<p>       查看日志，每次提交了什么： git log?</p>
<p>       其中commit 后面的b7dc85是版本号，可以进行版本号回退</p>

<p>       回退一个完整的版本：--hard，回退到上一个完整的版本</p>
<p>       git reset --hard HEAD~1??</p>
<p>       git reset --hard HEAD~2(回退两个版本)</p>

<p>       mixed回退到暂存区添加之前的状态，即add状态</p>
<p>       soft之后要么版本回退要么提交，退到commit状态</p>

<p>       回退到指定版本：git reflog</p>
<p>       git reset --hard b7dc854</p>

<p>11、其中origin可以替换，只是远程服务器的一个名字而已，</p>
<p>       git remote rename origin dev??</p>
<p>       git remote??</p>
<p>       返回dev??</p>
<p>       获取github项目的地址</p>

<p>12、克隆仓库：git clone</p>
<p>13、远程仓库重命名：git remote rename oldName newName(这步可改可不改)</p>
<p>14、添加源仓库地址为远程仓库： git remote add</p>
<p>15、查看文件夹： dir</p>

??
<p>差异比较：</p>
<p>16、比较工作区与暂存区： git diff ?</p>
<p>17、比较暂存区与本地版本库中最近一次commit 的内容： git diff --cached</p>
<p>18、比较工作区与本地版本库中最近一次commit的内容 ：git diff HEAD</p>
<p>19、比较两个commit之间的差异： git diff</p>

<p>基础工作流</p>
<p>20、查看分支： git branch ?</p>
<p>21、创建新分支： git branch ，新建完后要切换分支，然后add，commit，push，最后在github才有显示</p>
<p>22、创建并切换分支： git checkout -b</p>
<p>23、删除本地分支： git branch -d</p>
<p>24、删除远程分支： git push -d</p>
<p>25、切换分支： git checkout</p>
<p>26、删除某个文件： git rm -r --cached target ?删除target文件夹后commit，push到master</p>
<p>       master是装着没有bug的代码，dev分支是跟master一样的代码，但是允许报错</p>
<p>27、合并分支：git merge</p>
<p>28、把本地master分支推送到远程的master分支上：</p>
<p>       git push origin master:master</p>
<p>       git push origin master:dev</p>