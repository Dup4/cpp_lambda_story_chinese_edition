# C++ Lambda Story - From C++98 to C++20
## 介绍
本文为《C++ Lambda Story》的中文翻译，如果您觉得次数有价值，可以在 [https://leanpub.com/cpplambda](https://leanpub.com/cpplambda) 上支持下原作者。

或者如果您认识相关的翻译工作者或者出版社，可以积极联系原作者与出版社进行正规的中文翻译并出版。

## 目录

- [关于此书](Source/Chapter0/README.md)
    - [成书渊源](Source/Chapter0/README.md#成书渊源)
    - [阅读对象](Source/Chapter0/README.md#阅读对象)
    - [读者反馈](Source/Chapter0/README.md#读者反馈)
    - [代码证书](Source/Chapter0/README.md#代码证书)
    - [代码格式](Source/Chapter0/README.md#代码格式)
    - [语法高亮限制](Source/Chapter0/README.md#语法高亮限制)
    - [在线编译器](Source/Chapter0/README.md#在线编译器)
    - [关于作者](Source/Chapter0/README.md#关于作者)
    - [致谢](Source/Chapter0/README.md#致谢)
    - [校阅历史](Source/Chapter0/README.md#校阅历史)
- 一、[Lambda in C++98/03](Source/Chapter1/README.md)
    - [C++98/03 中的可调用对象](Source/Chapter1/README.md#1.-C++98/03-中的可调用对象)
    - [仿函数的一些问题](Source/Chapter1/README.md#2.-仿函数的一些问题)
    - [使用辅助函数](Source/Chapter1/README.md#3.-使用辅助函数)
    - [新特性的动机](Source/Chapter1/README.md#4.-新特性的动机)
- 二、[Lambda in C++11](Source/Chapter2/README.md)
    - [Lambda 表达式的语法](Source/Chapter2/README.md#1.-Lambda-表达式的语法)
        - [Lambda 表达式的一些例子](Source/Chapter2/README.md#Lambda-表达式的一些例子)
        - [Lambda 在编译器的展开](Source/Chapter2/README.md#Lambda-在编译器的展开)
    - [Lambda 表达式的类型](Source/Chapter2/README.md#2.-Lambda-表达式的类型)
        - [构造，还是拷贝？](Source/Chapter2/README.md#构造，还是拷贝？)
    - [调用操作符](Source/Chapter2/README.md#3.-调用操作符)
        - [重载](Source/Chapter2/README.md#重载)
        - [其他修饰符](Source/Chapter2/README.md#其他修饰符)
    - [捕获](Source/Chapter2/README.md#4.-捕获)
        - [`mutable` 关键字](Source/Chapter2/README.md#mutable-关键字)
        - [调用计数器 - 捕获变量的一个例子](Source/Chapter2/README.md#调用计数器---捕获变量的一个例子)
        - [捕获全局变量](Source/Chapter2/README.md#捕获全局变量)
        - [捕获静态变量](Source/Chapter2/README.md#捕获静态变量)
        - [捕获类成员和 `this` 指针](Source/Chapter2/README.md#捕获类成员和-`this`-指针)
        - [只能移动的对象](Source/Chapter2/README.md#只能移动的对象)
        - [保留常量](Source/Chapter2/README.md#保留常量)
        - [捕获参数包](Source/Chapter2/README.md#捕获参数包)
    - [返回类型](Source/Chapter2/README.md#5.-返回类型)
        - [尾部返回类型语法](Source/Chapter2/README.md#尾部返回类型语法)
    - [转化为函数指针](Source/Chapter2/README.md#6.-转化为函数指针)
        - [一个有趣的例子](Source/Chapter2/README.md#一个有趣的例子)
    - [IIFE - 立即调用函数表达式](Source/Chapter2/README.md#7.-IIFE---立即调用函数表达式)
        - [可读性提示](Source/Chapter2/README.md#可读性提示)
    - [Lambda 继承](Source/Chapter2/README.md#8.-Lambda-继承)
    - [在容器中存储 Lambda](Source/Chapter2/README.md#9.-在容器中存储-Lambda)
    - [总结](Source/Chapter2/README.md#10.-总结)
- 三、[Lambda in C++14](Source/Chapter3/README.md)
    - [为 Lambda 增加默认参数](Source/Chapter3/README.md#1.-为-Lambda-增加默认参数)
    - [返回类型](Source/Chapter3/README.md#2.-返回类型)
    - [带有初始化的捕获](Source/Chapter3/README.md#3.-带有初始化的捕获)
        - [限制](Source/Chapter3/README.md#限制)
        - [对现有问题的改进](Source/Chapter3/README.md#对现有问题的改进)
    - [泛型 Lambda](Source/Chapter3/README.md#4.-泛型-Lambda)
        - [可变泛型参数](Source/Chapter3/README.md#可变泛型参数)
        - [使用泛型 Lambda 进行完美转发](Source/Chapter3/README.md#使用泛型-Lambda-进行完美转发)
        - [减少一些隐蔽的类型纠正](Source/Chapter3/README.md#减少一些隐蔽的类型纠正)
    - [使用 Lambda 代替 std::bind1st 和 std::bind2nd](Source/Chapter3/README.md#5.-使用-Lambda-代替-std::bind1st-和-std::bind2nd)
        - [使用现代 C++ 技术](Source/Chapter3/README.md#使用现代-C++-技术)
        - [函数组合](Source/Chapter3/README.md#函数组合)
    - [Lambda 提升（LIFTing with Lambda）](Source/Chapter3/README.md#6.-Lambda-提升（LIFTing-with-Lambda）)
    - [递归 Lambda](Source/Chapter3/README.md#7.-递归-Lambda)
        - [利用 std::function](Source/Chapter3/README.md#利用-std::function)
        - [内部 Lambda 和泛型参数](Source/Chapter3/README.md#内部-Lambda-和泛型参数)
        - [更多技巧](Source/Chapter3/README.md#更多技巧)
        - [使用递归 Lambda 是最好的选择吗？](Source/Chapter3/README.md#使用递归-Lambda-是最好的选择吗？)
    - [总结](Source/Chapter3/README.md#8.-总结)
- 四、Lambda in C++17
    - Lambda 语法更新
    - 类型系统中的异常规范
    - constexpr Lambda 表达式
    - 用例
    - 捕获变量
    - constexpr 总结
    - 捕获 *this
    - 一些指导性意见
    - IIFE 更新
    - 可变泛型 Lambda 的更新
    - 从多个 Lambda 派生
    - 自定义模板参数推导规则
    - 聚合初始化的扩展
    - std::variant 和 std::visit 的例子
    - 使用 Lambda 进行并发编程
    - Lambda 和 std::thread
    - Lambda 和 std::async
    - Lambda 和 C++17 的并行算法
    - Lambda 和异步 - 总结
    - 总结
- 五、Lambda in C++20
    - Lambda语法更新
    - 更新快览
    - consteval Lambda
    - 捕获参数包
    - 模板Lambda
    - Concept和Lambda
    - 无状态Lambda的变更
    - 补充一些关于“未评估的concept”
    - Lambda和 constexpr 算法
    - C++20 对重载模式的更新
    - 总结
- 附录A - 技术名录
- 附录B - 五大使用C++ Lambda的优势
- 参考
- 笔记

## 致谢
本书 Chapter 4 C++17 章节翻译感谢 [@Dup4](https://github.com/Dup4) 同学的支持。
