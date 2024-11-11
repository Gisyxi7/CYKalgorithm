# CYKalgorithm

## 功能
输入一个字符串和一个上下文无关文法，输入格式必须为**Chomsky标准形式**！！！

For example：

$\omega=ababa$

$S\rightarrow AB,A\rightarrow BC|a,B\rightarrow AC|b,C\rightarrow a|b$

判断该字符串是否属于该文法定义的语言。
## 用法
通过以下函数输入字符串和文法。
```
void initialize()
```

用宏定义控制是否输出调试信息。
```
#define DEBUG
```
### 文本输入
## 限制
文法输入格式必须为Chomsky标准形式，即每个产生式都满足以下两个形式的其中一种。
1. $A\rightarrow BC$，产生式体是两个变量。
2. $A\rightarrow a$，产生式体是一个终结符。

推荐只用A-Z代表变量，a-z代表终结符。

默认S是起始符号。

默认在变量不超过5个时调试信息输出对齐。

默认字符串长度不超过10，超过时调试信息输出下标可能会看着有点奇怪。

