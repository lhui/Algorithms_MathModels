===============================================================
               遗传算法求TSP问题MatLab程序说明
===============================================================
本程序是配套于本人的 <MCM中常用数法之启发式算法> 课程. 由于是美
赛课程, 以及本人编程的风格, 程序中的注释采用英文. 现对程序作一
简要中文说明：

main.m           主程序. 主程序中有一rand('seed',n) n 为某一整
                 数, 这是设置随机数发生器的种子，这样实际上规定
                 了随机数发生的方式，因此后面的随机数其实都是定
                 下来的，这样所有人就可以看到同一结果, 可注释掉
                 此行，那么每次的结果就不一定再相同了. 

distancematrix.m 这个函数用于生成距离矩阵.

select.m         选择操作, 提供了两种选择方式：轮盘赌和两两竞争

crossover.m      交叉操作

mutation.m       变异操作
  
plotcities.m     画中国地图, 及城市, 并生成初始路径句柄.

plotroute.m      画新路径, 并显示距离和温度.

totaldistance.m  计算每条路径的总距离. 这个函数中调用了distance
                 函数用于求球面距离. 由于个别同学说他们的matlab
                 中不函此函数, 我在本函数下补了一个简单的求球面
                 距离的函数distance.

fpdfprinter.m    这个程序是经xu junjie的程序略作修改而来, 用于输
                 出页边距合适的pdf图片.

===============================================================

作者：周吕文, zhou.lv.wen@gmail.com

2012.11.11
===============================================================

