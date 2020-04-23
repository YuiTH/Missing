# Ep.1 shell

1. 在/tmp文件夹下创建一个叫做missing的文件夹
2. 查查touch命令是做什么用的，可以考虑使用man命令
3. 用touch在missing下创建一个叫做semester的文件
4. 在一个文件里写这么两行：
```sh
 #!/bin/sh
 curl --head --silent https://missing.csail.mit.edu
 ```
  第一行的意思出刊可能会比较费解，#开头在bash里表示注释。这个开头你可能在许多Python脚本里也见过。执行这个文件（./semester）思考为什么启动不了？可以考虑用ls -l看看文件属性

5. 通过手动指定解释器来启动这个脚本，比如sh semester为什么这样可以启动而直接./文件名却不行？
6. 查查看chmod程序（记得可以用man）
7. 用chmod使得刚刚的脚本可执行，思考为什么这样就能执行了？shell从哪里知道使用哪个解释器来运行的？