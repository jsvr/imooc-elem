## git冲突

### git 本地和远端冲突

```
1. 报错信息
error: Your local changes to the following files would be overwritten by merge:
	.idea/workspace.xml
	copy-imooc-elem/config/index.js
Please commit your changes or stash them before you merge.
2. 解决办法
   使用git checkout 可以丢掉本地的改动,然后使用git pull去拿server上的最新更新.
```