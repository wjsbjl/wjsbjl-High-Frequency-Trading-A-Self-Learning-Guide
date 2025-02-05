- 出现了`.h`文件
	- 声明函数，类，全局变量
	- 包括function prototypes, class definitions，constants, and macros
	- `.h`说明做什么，`.cpp`说明怎么做
	- 编译的时候，`.h`文件出现在一开始的`#include "perfect.h"`中的预处理阶段，起到定义和函数prototype的作用。多个include冲突的时候可以`#ifdef, #define, #endif`来操作。

## Stack Overflow
- 程序调用函数时，计算机为该函数调用分配内存，称为栈帧（stack frame），被存在调用栈（call stack）中，每次调用都会创建一个新的栈帧（python的debug尝看到）
- 递归调用过深导致栈溢出，数据量过大可能也会导致。
- 理解为栈帧调用过深，一个**不会结束的 `for` 或 `while` 循环**通常是不会直接导致 **栈溢出**（stack overflow）的，因为栈溢出是由递归调用引起的，而不是循环。

## **onlyConnectize**
- 没有递归解决问题的思路，参考了[知乎](https://zhuanlan.zhihu.com/p/463263796)的内容。递归用的很少，基本思路就是把问题细分到最小单位，后续再多理解下。
- 对于debug，断点打了以后在变量框看结果，有一点python里面用debug的感觉了
- test挺有意思的，直接运行会核对答案
- ==写完才往下读文档，其实很多内容文档都提到了，最好看完一整道题再写==
## **Sandpiles**
- ==不理解为什么Grid后面要加\<int\>==，
	- **Data types** define the nature of the data and the operations that can be directly performed on such data.
	- **Template classes** provide a mechanism to define classes or functions that can work with any type, promoting code reusability and flexibility. They are not types themselves but are used to generate types.
	- You might have noticed that the first argument is a **Grid\<int\>**, a type we haven’t encountered before. This is a type representing a fixed-size, two-dimensional grid of integers, like the grids that we showed on the previous pages.
- 位置搞错了，整成四个角的位置了
- 变换顺序不会影响，一开始以为必须要同时处理四个位置

## **Plotter**
