### Git Commands:
- 显示所有日志  
```git log -a ```
- 对于错误add 还未commit
  1. Option 1: 不删除物理文件，仅将该文件从缓存中删除    
    ```git rm <-r, recursive>--cached <文件路径> ```   
  2. Option 2: 不仅将该文件从缓存中删除，还会将物理文件删除（不会回收到垃圾桶）   
    ```git rm --f  <文件路径>```
- 对于错误commit，还未push
  1. Step 1: 回滚到上一次commit，此时上一次add还未撤销   
    ``` git reset soft HEAD~1```   
  2. Step 2: 撤销上次add，随后可以重新add && commit then push   
    ```git reset --mixed```
- 修改和查看远程仓库地址   
  1.  ```git remote -v```   
  2.  ```git remote set-url origin <remote url>```