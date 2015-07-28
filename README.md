#LDPC码误码率的蒙特卡罗仿真
代码内包含基本的LDPC码编码器，译码器实现方式，以及BPSK通信系统的基本仿真原理（AWGN信道）。这被用来实现LDPC码误码率的仿真，同时也是我托管在GitHub上的第一份代码，用于学习GitHub的使用。
代码的更多说明可参见我的[博客](http://www.cnblogs.com/sea-wind2)。
----
说明详见主分支。这一分支对最小和译码算法进行了优化，具体表现在去掉了一重循环，改用矩阵实现。这一优化的代价是使得译码算法只能够用在CCSDS提及的LDPC码上，即对校验矩阵的结构有具体的要求。这一修改在运行速度上的提升是显著的，运行速度最快可提高近20倍。