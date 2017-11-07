#Python3.6&&numpy

### 1. source

* [provided by cs231n](http://cs231n.github.io/python)
* [official doc](https://docs.python.org/3.6/tutorial/index.html)

### 2.notes

* +-\*作用没变,\*\*可以计算幂,/是浮点数，//是整除

* _在交互界面中代表上次的输出结果

* 可以用\_\_doc\_\_访问函数的documentationStrings,自己写的时候要按照一定规范写在函数的第一行

* 函数里参数的初始值只会**初始化一次**，例如

    ```python
  def f(a, L=[]):
  	L.append(a)
  	return L

  print(f(1))#[1]
  print(f(2))#[1, 2]
  print(f(3))#[1, 2, 3]
    ```

* 传参的时候，keyword argument后面必须都是keyword argument

* 可以用

    ```python
  def cheeseshop(kind, *arguments, **keywords):
    ```
    来传list参数和dict参数