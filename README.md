# 天津津南工艺优化
[天池津南数字制造算法挑战赛【赛场一】链接](https://tianchi.aliyun.com/competition/entrance/231695/introduction)
### 任务介绍：
1.以异烟酸生产过程中的各参数，包括各主要步骤的时间、温度、压强等参数为基础,对收率进行预测。   
2.基于自身训练的模型，找到最佳收率的参数组合。即使得模型预测值到达最大（收率不能超过1）


### 文件说明：
#### 1.使用贝叶斯优化，搜索最优工艺参数  
model_evaluate.py # 对每一轮搜索的参数进行收率计算   
explore_optima.py # 搜索最优工艺参数 

#### 2.对收率进行预测   
train_data.py  # 整合之前的测试集和训练集 
model_FuSai.py # 预测复赛测试集 FuSai.csv   
model_optimize.py # 预测最佳收率的组合 optimize.csv   
run.py # 依次运行上述文件 
