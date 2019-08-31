# playML
基于Numpy&Python模拟scikit-learn实现基本的Machine Learning算法
其中主要包括：
- KNN
- Simple Linear Regression
  - [使用简单线性回归预测Boston房价与房间数量的关系](https://github.com/jeremybaby/playML/blob/master/02_linear_regression/03_measure_and_predict_Boston_house_data.ipynb)
    - 评价指标: MSE RMSE MAE R^2
  - [使用多元线性回归预测Boston房价与13个属性的关系]()
    - 方法：使用Normal Equation进行预测
        - 缺点：时间复杂度为O(n^3)(优化后为O(n^2.4))
    - 评价指标：
        R^2 = 0.8129794056212832
    - [系数矩阵的可解释性](): 
        - 正相关影响最大的因素
          - RM 代表房间数量【房间数量越多，价格越高】
          - CHAS 是否临近Charles River，临河为1，不临河为0【“河景房”价格越高】
        - 负相关
          - NOX 房屋周边CO浓度【CO浓度越高，房价越低】
          - DIS 距离Boston5个人才市场加权平均的距离【距离越小，房价越高】
        - More
          - 关于RM，可否进一步采集房屋面积、房型、楼层等数据，进一步得到更好效果
          - 关于NOX，可否进一步采集房屋附近的化工厂、排放数据等进一步判断房屋的价格 
- Gradient Descent
- PCA
- 多项式回归
- 逻辑回归