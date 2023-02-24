### 0x00 关于

当前目录用于收录阅读相关书籍过程中的一些外链读物资料。

收录资料的同时，在相 0x01 相关的部分中会记录相应的收获点。

## 0x01 目前收录

<details><summary>tutorial of opcode by svin</summary>
<p>

#### quiz 1: What "opcode" is?


>   以指令 lodsb 为例进行说明，其对应的 opcode 是 ACh，处理器并不懂 lodsb 的含义，
lodsb 只是作为 ACh 操作码的助记符，是用于指示编译器在编译过程中遇到 “lodsb” 会在你的文件中插入对应的值（ ACh ）。

<hr> 
#### quiz 2: 如何将存在的 opcode 和其对应的助记符对应？
> 最方便的方法--通过 ollydbg
<img width=900 src="https://user-images.githubusercontent.com/89090949/221190780-1be36777-892a-454f-bfe5-336d30ef7d6f.gif"></img><br>
随意载入一个程序，选中某行，enter 进行编辑， 输入内容 lodsb 完成指令覆写， 中间列 ollydbg 指示出助记符 lodsb 对应的 opcode 为 AC，验证方法使用 ctrl + e 输入 opcode ACh <br>
<img width=900 src="https://user-images.githubusercontent.com/89090949/221191907-bceaa9bb-dd5b-402f-86fc-2adbd3d6e4fb.gif"> <br>
二者一致
<hr> 

#### quiz 3: 是否 opcode 和助记符都是 1 V 1的关系？
> <img width=900 src="https://user-images.githubusercontent.com/89090949/221193018-635e9a33-6c80-4e07-ba8c-b41343ee75a4.gif"><br>
 助记符 nop 和 xchg eax,eax 的 opcode 一致，再比如：<br>
 <img width=900 src="https://user-images.githubusercontent.com/89090949/221193401-147dc9b3-c928-4dd1-a249-2b8d2b7e3c61.gif"><br>
 助记符 `add eax,1` 的 opcode 同指令序列 `05 01 00 00 00` 一致, 但指令长度不一样，一个3字节 一个 5字节

<hr> 

> 有点流水账...

</p>


![121]()


![121]()
