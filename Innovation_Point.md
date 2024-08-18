# 用于记录平时出现的idea

1. 基于Transformer架构的话，可以研究一下位置信息的编码加入，这是目前预测的主要问题所在

2. 创新点估计：
   - 深度学习的预测部分可以把trend-cycling和seasonal的部分区分开来做，都提供给Online Optimization
   - 结合Online和DL的部分会是一个另外的创新点，这一部分还需要进一步优化
   - 在多个benchmark上面做了extensive experiment，可以作为第三个创新点

3. 深度学习初步创新点：
   - 因果膨胀卷积(WaveNet)替代原来的isometric convolution
   - 加权求和
   - 对于时序休息的空间域和频域的信息分别提取
   - 大概率会完全使用卷积来做，而不采用Transformer架构
   - 不仅仅考虑时间域的信息，同时结合频域的信息，结合在一起，从而达到更加好的提取效果

5. 在线优化结合创新：
   - 以nuips论文提出的观点为baseline，设置一个系数从而达到效果
