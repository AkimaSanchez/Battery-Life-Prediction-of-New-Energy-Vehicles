# 基于LightGBM模型的新能源汽车电池寿命预测
## Battery-Life-Prediction-of-New-Energy-Vehicles

### 写在前面
该项目正在进行，所以先不给相关的资料。  
This project is still in progress, so I won't provide the relevant materials for now.  

针对SOH评估问题，本研究以CALCE数据集中的锂钴氧（LiCoO₂）电池为对象，提出了一种基于LightGBM的SOH预测方法。通过K-Means聚类算法结合线性插值法处理异常值，筛选出恒压充电时间（CVCT）、循环次数、电池内阻（IR）等12项关键指标，并利用皮尔逊相关系数验证其与SOH的强相关性（|r|>0.7）。构建的LightGBM模型经贝叶斯优化调参后，在测试集上表现出色，优于随机森林（RandomForest）和XGBoost等对比模型。  
This study focuses on the State of Health (SOH) evaluation problem of lithium cobalt oxide (LiCoO₂) batteries in the CALCE dataset and proposes a SOH prediction method based on LightGBM. By using the K-Means clustering algorithm combined with linear interpolation to handle outliers, 12 key indicators such as constant voltage charging time (CVCT), cycle count, and internal resistance (IR) of the battery are selected. The strong correlation (|r|>0.7) between these indicators and SOH is verified by Pearson correlation coefficient. After Bayesian optimization for parameter tuning, the constructed LightGBM model performs excellently on the test set, outperforming comparison models such as RandomForest and XGBoost.

数据处理主要思路由：[XiuzeZhou大佬](https://github.com/XiuzeZhou/CALCE)、[戏作三味大佬](https://blog.csdn.net/qq_66826153/article/details/146908606)提供
