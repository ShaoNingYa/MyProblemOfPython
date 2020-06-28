# MyProblemOfPython

## Problem1——test001

关于python导包的问题，我的目录结构是：

- test
  - testa
    - min.py
    - util.py
  - testb
    - min.py
    - util.py
  - main.py

在main.py中会分别调用testa和testb中的min.py，输出对应内容，然后再min.py中也会导入自己目录下的util，但是如果直接进行导入的话，去执行main.py就会报错，说找不到util模块，因此，再min.py中加入了`sys.path`用来导入，这样确实可以执行了，但是又有新的问题，他们所引用的util.py文件是同一个，我的设想是testa中的util和testb中的util是不同的，当前这个问题不知道应该怎么解决。