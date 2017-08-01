十六进制数由 0~9 及 a~f 共16个字符组成，其中 a~f 分别表示 10~15。假设有16进制数0eaf，其转换为十进制数的计算方法为：0×163 + 14×162 + 10×161 + 15×160，结果为 0+ =3759。这个结果可以用Windows自带的计算器加以验证。

一、	用户界面

![](/図1.png)

二、代码

![](/図2.png)

![](/図3.png)

![](/図4.png)


程序非常简单，但是在制作过程中将16进制数的字符串分解为列表时，出现了异常情况。注意到，在Hex转Dec的过程中，循环变量的起始值是2，而不是1，原因是AppInventor在将一个字符串（如"eaf"）用空字符（""）作为分隔符分解为列表时，列表的长度本应为3，列表元素为（eeaf），但实际上分解后所得列表的长度为4，其中列表的第一个元素为空字符，即列表为（"", e, a,f），这是开发工具本身的bug，为了获得正确的结果，只能忽略列表的第
![](/333.png)
https://drive.google.com/file/d/0By3vhVxl2nhlM0JMSGlxZ01rU1U/view?usp=sharing
