# 练习和编程

1. 有这样一个问题：一个列表，比如是[1, 2, 3]，在最右边增加一个数字。显然使用列表的append方法追加元素。

```
    >>> lst = [1, 2, 3]
    >>> lst.append(4)
    >>> lst
    [1, 2, 3, 4]
```

再进一步，能不能在最左边增加一个数字呢？比如在列表的左边增加整数7，或许下面的是一种方法：

```
    >>> nl = [7]
    >>> nl.extend(lst)
    >>> nl
    [7, 1, 2, 3, 4]
```

除了这种方法之外，Python标准库collections中提供了一个名为deque的模块。

```
>>> from collections import deque
```

请根据已经学习过的知识技能，研究deque（翻译为“双端队列”）的使用方法。

然后使用deque，解决下属问题：

自定义一个固定尺寸的缓存对象，当它被填满的时候，新加入一个元素后，第一元素，也就是最老的那个元素要被删除。

2. ScriPy是一个非常好的用于做“爬虫”的第三方包，请访问其官方网站，并在本地计算安装，然后自己选定网站，用ScriPy做爬虫，获取选定网站的有关内容。