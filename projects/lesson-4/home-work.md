### 思考如何能覆盖所有的测试路径:

1. 先看函数声明

先测试正确调用

再从控制变量的角度测试各`参数`的合法性, 各 `modifier` 条件是否满足, 各`返回值`是否正确

2. 从函数功能的维度

看功能上是否允许重复调用

测试函数体内各断言语句

3. 异常捕捉

尽量在所有可能地方捕捉异常