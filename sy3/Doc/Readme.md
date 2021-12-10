
# C 语言关键字 - volatile

    根据 volatile 修饰符的特性，构造一个程序（主程序、中断子程序的程序结构）。要求：无 volatile 时，程序会出现随机的运行逻辑错误。加入 volatile 后，程序随机的运行逻辑错误消失。

## 实验原理

- 两个变量

        char (volatile) cValue1;
        char (volatile) cValue2;

- 运行流程

        若是变量 cValue1 没有声明 volatile，则与之相关 if 的判断语句不成立。
        反之，按下多次按键1使 cValue1 递增，则会进入无限循环，输出打印USART1 is ready...
        变量 cValue2 同理。

# 参考资料

    KEIL里 Volatile的用法
    https://blog.csdn.net/djimon/article/details/7804951

    keil编译器的优化问题 关键字volatile的使用
    https://blog.csdn.net/weixin_42916705/article/details/102677496
