### ubuntu操作：
- 添加环境变量：
	1. ```vim ~/.bashrc ```
	2. 在文件末尾添加路径： ```example: export PATH=~/dependency/kenlm/build/bin:$PATH```
	3. ```source ~/.bashrc``` //加载一下 
	4. 查看已添加环境变量，使用“：”隔开：```echo $PATH ```  
	
- 寻找文件地址：  
    ```which <filename>```
    
- 打印pip包路径：  
    ```pip2 show <package name>```
    
- 查看用户：  
    ```sudo cat /etc/shadow```
    
- npm项目忽略module push到github:
    1. ```vim .gitignore``` //创建用于忽略某些文件的文件
    2. 写入要忽略的文件，如：```node_modules/```
    3. ```git add . $ git commit -m "xxx" & git push```
    
- 操作远程ssh终端：  
  ```source activate <env name>``` //激活某python环境  
  ```cat /usr/local/cuda/version.txt``` //查看CUDA版本

- 当win中.sh复制到linux，需要修改文件格式
  ```
  vim <file> 
  :set fileformat=unix
  wq
  ```
- 设置文件为可执行文件
  ```chmod +x <file>```
