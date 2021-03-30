# GE2E-speaker_recognition
基于广义端到端网络（GE2E）思想实现，复现的github上的代码，采用VCTK数据集，VOX1,2也可以用，做些修改即可。

# 安装环境
pip install -r requirements.txt

# 准备数据
本实验采用VCTK数据集，也可以采用Voxceleb1，Voxceleb2，Aishell等数据集，只需在data_preprocess.py做相应修改即可

# 配置参数
configuration.py为参数配置文件，包含是否训练，训练批次大小，每个批次的说话人个数，每个人的话语数，LSTM网络结构等参数

# 训练
train.py  配置好环境之后，准备好数据并配置好参数之后即可进行训练

# 测试
test.py   用于测试。

# util
工具类，用于计算EER，相似度矩阵等的定义

# 该实验包括文本相关说话人识别 和 文本无关说话人识别

本实验评价指标为EER，在VCTK上EER结果为9%左右。
