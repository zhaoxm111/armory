![0](/Users/easemob/Desktop/0.png)

#### 获取代码库

##### 1 、 fork别人的仓库到自己的GitHub

![1](/Users/easemob/Desktop/1.png)

##### 2、将fork到的仓库clone到本地local

![2](/Users/easemob/Desktop/2.png)

#### 同步更新代码

因为fork并不能将所有东西都复制过来，这部操作只是获取到了路径，所以此时local仓库和upstream远程仓库并不同步，想同步需要fetch

##### 3、使A local仓库和远程upstream仓库的master分支同步

```
$ git fetch upstream
$ git rebase upstream/master
```

##### 4、A在本地对代码进行修改之后，在SmartGit进行commit提交操作，然后push到自己的origin仓库

![3](/Users/easemob/Desktop/3.png)

```
$ git push origin master
```

##### 5、去GitHub提pr

![4](/Users/easemob/Desktop/4.png)

![5](/Users/easemob/Desktop/5.png)

![6](/Users/easemob/Desktop/6.png)

到此就已经完成了所有操作，如果原作者同意你的pr申请，你就成功的对upstream的代码进行了修改

##### 6、B想要更新到upstream仓库的最新版本，就必须在终端进行fetch,rebase等操作(同上3)

##### 7、B的local仓库已同步,需要将最新版本push到B自己的origin仓库,使origin仓库更新