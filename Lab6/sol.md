## ex1
太困了 我就用中文写了。

> In `OUT4`, if we decide to find the negative input with 2's complement format. What the output of this format ?

如果最高位（第[8]位）是1：次高位（第[7]位）是0则说明是负数输入；  
如果最高位（第[8]位）是0：次高位（第[7]位）是1则说明是负数输入。  
所以说，观察最高位、次高位，若不一样，则是负数输入。

## ex3
> How to automatic set the reset signal in this circuits ?

利用 CLK + Adder + 寄存器 的方法（类似lab5第2题），从0开始每次加1，加到一定值后（使用比较器判断）（这就是周期），输出1信号至RST，并调用寄存器的reset清空。  
我猜是这样的？因为太语焉不详了，我搞不懂什么是 `automatic` .

> Can you use sequential circuits only to implement such circuits ?

移位寄存器 may work. 但我不会用😭