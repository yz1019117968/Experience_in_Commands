### Win Commands:
- 将test1中文件夹复制到test2中： 
    `xcopy d:\test1  d:\test2 /T /E`  
- 批量转文件后缀:  
    ```
    @echo off 
    for /d %%i in (D:\Projects\funcs_comments_v11122020_backup\*) do ( 
            cd %%i 
            ren *.txt *.sol
            )
    ```
- 查看当前文件夹下全部文件： `dir /a *`
- 删除某个文件： `del <file name>`
- pytorch 查看cuda, cudnn版本:
	```
    import torch
	print(torch.__version__)
	print(torch.version.cuda)
	print(torch.backends.cudnn.version())
    ```