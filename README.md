# HorseRace-Animation
利用定位马left值和页面滚动实现赛马动画
预览：[https://leeseean.github.io/HorseRace-Animation](https://leeseean.github.io/HorseRace-Animation)

实现原理：
    跑的路程distance固定一个数字，按约定好的排名给出每匹马需要跑的时间，第一名的时间最短，最后一名时间最长。
    将跑的路程分段，随机一个时间来确保每一段速度不同，保证总的时间在约定好的时间之内。
    如15000米，可分成3个500米，每段时间比例[0.45,0.35,0.2](相加保证为1)，则其中一速度v = 500/0.45*总的时间，其他两个速度也是同样的公式。
