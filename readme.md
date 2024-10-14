# 算法竞赛入门——语法

## 环境要求

- Dev Cpp 5.11（校赛环境，务必要使用过，OJ首页有提供下载链接）
- [进一步了解环境](https://www.cnblogs.com/Fighoh/p/18086412)

## 第一份代码

```c++
#include <bits/stdc++.h>

using namespace std;

int main() {
    cout << "Hello World!\n";
    return 0;
}
```

这里大致分为三部分

- 头文件 `#include <bits/stdc++.h>`

  简单来说就是写上某个头文件之后就可以使用某些函数或者类型，比如代码中的`cout`其实是包含在`<iostream>`这个头文件里面。

  但是在我们**算法竞赛**中，为了追求方便，我们可以使用一个包含了绝大多数你会用到的函数或者类型的头文件——万能头`#include <bits/stdc++.h>`，这样就不用写其余头文件了

- 命名空间`using namespace std;`

  就是使用`std`这个命名空间，主函数的`cout`其实是在`std`这个命名空间当中，如果不加这行代码我们调用`cout`，就需要写成`std::cout`，简单来说就是让我们写代码的时候少写一部分内容

- 主函数`int main() {}`

  包含两部分内容

  - 程序的主体`cout << "Hello World!\n";`
  - 函数的返回值`return 0;`

**总而言之**，我们编写代码的总体框架就是（**仅限于算法竞赛**！！！课堂请按老师要求书写）

```c++
#include <bits/stdc++.h>

using namespace std;

int main() {
    /*
    程序的主体内容
    */
    return 0;
}
```



## 输入输出

```c++
// c风格输入输出
int a;
scanf("%d", &a);
printf("%d", a);

// c++风格输入输出
int a;
cin >> a;
cout << a;
```

以上列举了`c`和`c++`风格的输入输出，



















# 附录

## 头文件

通常用于声明函数、类、结构体、宏等，以便在多个源文件中使用。头文件的扩展名通常为`.h`或`.hpp`。

**输入/输出流**

- `#include <iostream>`：用于输入输出操作，`cin`和`cout`等功能。
- `#include <iomanip>`：用于控制输入输出格式，例如控制小数点位数。

**容器类和算法**

- `#include <vector>`：动态数组容器。
- `#include <array>`：静态数组容器。
- `#include <list>`：双向链表。
- `#include <deque>`：双端队列。
- `#include <map>`：关联容器，存储键值对。
- `#include <set>`：无序、不重复的集合。
- `#include <algorithm>`：提供排序、搜索等算法。
- `#include <iterator>`：用于操作迭代器。

**字符串处理**

- `#include <string>`：用于操作C++的`std::string`类。
- `#include <cstring>`：用于C风格字符串的操作函数，如`strcpy`，`strcmp`。

**数学库**

- `#include <cmath>`：数学函数库，包含`sin`，`cos`，`sqrt`等函数。

## C++ 关键字

下表列出了 C++ 中的保留字。这些保留字不能作为常量名、变量名或其他标识符名称。

| asm          | else      | new              | this     |
| ------------ | --------- | ---------------- | -------- |
| auto         | enum      | operator         | throw    |
| bool         | explicit  | private          | true     |
| break        | export    | protected        | try      |
| case         | extern    | public           | typedef  |
| catch        | false     | register         | typeid   |
| char         | float     | reinterpret_cast | typename |
| class        | for       | return           | union    |
| const        | friend    | short            | unsigned |
| const_cast   | goto      | signed           | using    |
| continue     | if        | sizeof           | virtual  |
| default      | inline    | static           | void     |
| delete       | int       | static_cast      | volatile |
| do           | long      | struct           | wchar_t  |
| double       | mutable   | switch           | while    |
| dynamic_cast | namespace | template         |          |