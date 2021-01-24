# myReverseExps

> By c10udlnk

一些逆向常用脚本&&常见加密的收录。

P.S. 鲁棒性不强，请保证输入都是规范的，不然输出有问题就不是我的锅（逃。

持续更新ing...

## 逆向

### SMC

处理异或的SMC文件时的patch脚本，在IDA中File->Script file，导入脚本运行即可。

- `patch_SMC.py`：patch脚本，需修改相应的codeStart（smc起始地址）、codeLen（长度）和xorData（用来xor的key）。

### Angr

运用[angr](https://c10udlnk.top/2020/11/11/logFor-Angr-CTF/)爆破某些二进制文件。

- `myAngr.py`：angr脚本，需修改path_to_binary（文件路径）和相应参数（比如find_address之类的）。

### Brainfuck

将Brainfuck源码转换为易懂的C或者python代码，在`bfCode.bf`中输入brainfuck代码，运行相应的文件即可。

建议转换为C，相比之下Python在处理char型数据时会冗杂很多。

另外C++和C差不多就不另写了（

- `bfCode.bf`：[Brainfuck](https://en.wikipedia.org/wiki/Brainfuck)源码。

- `brainfuck2c.py`：将Brainfuck转换为C语言代码，存入`res.c`中。

- `brainfuck2py.py`：将Brainfuck转换为python代码，存入`res.py`中。

## 加解密

（……）