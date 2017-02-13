1. 最近常用到git来push代码到origin development分支上，也出现了几次vim窗口，防止忘记还是记录下来比较好；

2. 首先按ESC键退出编辑状态，然后按shift+;键，再按wq!保存退出，按q!则为不保存退出；

3. 建议大家在编辑或者修改代码之前先pull一下oirign的代码，在push之前也要pull一下代码，可以减少一些不必要的麻烦。当然也可以按下面的操作先保存操作，pull之后再把保存的恢复。

> 步骤如下
1. 先将本地修改存储起来   
	```git stash```   
	这样本地的所有修改就都被暂时存储起来。   
	用git stash list可以看到保存的信息，   
	显示的内容：stash{0}:WIP on master:a80c24d          打印系统环境变量
	其中stash{0}就是刚才保存的标记。
2. pull内容   
	暂存了本地修改之后，就可以pull了
	```git pull```  
3. 还原暂存的内容   
	```git stash pop stash@{0}```   
	系统提示如下类似的信息：   
	Auto-merging c/environ.c
	CONFLICF (content):Merge conflict in c/environ.c   
	意思就是系统自动合并修改的内容，但是其中有冲突，需要解决其中的冲突


