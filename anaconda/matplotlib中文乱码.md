# matplotlib中文绘图中x,y label 乱码

## linux：

### 			安装windows字体

   + 从windows的C盘中C :\ windwos\Fonts 复制其 内容，在/usr/share/fonts 中新建文件夹 windowsfonts 

   + 运行 sudo fc-cache -fv 刷新字体

     

### 			jupyter 配置绘图字体



``` python
import matplotlib.pyplot as plt
plt.rcParams['font.sans-serif']=['Microsoft YaHei'] #用来正常显示中文标签
plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
plt.plot([1,2,3,4,5])
plt.xlabel('x轴，测试测试')
plt.show()
# 先用这个代码测试 Microsoft YaHei 是否安装
```

- 若无问题，修改matplotrc文件

``` python
import matplotlib
matplotlib.matplotlib_fname() #将会获得matplotlib包所在文件夹
```

- 将matplotlibrc文件内的font.family修改为Microsoft YaHei

``` python
# 例如一下
font.family         :Microsoft YaHei
```

- 重启后测试绘图

``` python
import matplotlib.pyplot as plt
plt.plot([1,2,3,4,5])
plt.xlabel('x轴，测试测试')
plt.show()
```

