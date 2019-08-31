# playML
基于 **Numpy** & **Python3** 模拟scikit-learn实现基本的Machine Learning算法
- **playML**目录下为独立封装的Machine Learning算法
## How to Use
 ```python
from playML.LinearRegression import LinearRegression
reg = LinearRegression()
reg.fit_normal(X_train, y_train)
 ```
<hr/>

### 1. KNN
  - **Feature**
    - 非参数学习
    - 可解决分类与回归问题
    - 对数据没有假设
### 2. Linear Regression
  - **Feature**
    - 典型的参数学习
    - 只能解决回归问题
    - 对数据有假设：线性
  - [使用简单线性回归预测Boston房价与房间数量的关系](https://github.com/jeremybaby/playML/blob/master/02_linear_regression/03_measure_and_predict_Boston_house_data.ipynb)
    - **Method**：[求偏导数得到的极值点](https://github.com/jeremybaby/playML/blob/master/playML/SimpleLinearRegression.py)
      - 优化: 向量化
    - 评价指标: 
        - MSE RMSE MAE 
        - R^2 = 0.6129316803937324
  - [使用多元线性回归预测Boston房价与13个特征的关系]()
    - **Method**：[Normal Equation](https://github.com/jeremybaby/playML/blob/master/playML/LinearRegression.py)
        - 缺点：时间复杂度为O(n^3)(优化后为O(n^2.4))
    - **评价指标**：
        - R^2 = 0.8129794056212832
    - **Result**：[系数矩阵的可解释性](https://github.com/jeremybaby/playML/blob/master/02_linear_regression/05_mulpitle_linear_regression_in_scikit-learn.ipynb)
        - **正相关**
          - RM 代表房间数量【房间数量越多，价格越高】
          - CHAS 是否临近Charles River，临河为1，不临河为0【“河景房”价格越高】
        - **负相关**
          - NOX 房屋周边CO浓度【CO浓度越高，房价越低】
          - DIS 距离Boston5个人才市场加权平均的距离【距离越小，房价越高】
        - More...
          - 关于RM，可否进一步采集房屋面积、房型、楼层等数据，以更好地判断房屋价格
          - 关于NOX，可否进一步采集房屋附近的化工厂、排放数据等以更好地判断房屋的价格 
### 3. Gradient Descent
<hr/>

### 4. PCA
<hr/>

### 5. 多项式回归
<hr/>

### 6. 逻辑回归
<hr/>
