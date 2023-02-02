# 比赛
[OTTO competition 2022](https://www.kaggle.com/competitions/otto-recommender-system/leaderboard)


简单来说是一个纯用户行为交互的比赛，预测三种用户行为，click/cart/order

# 关键上分点：
1. co-visitation矩阵
2. ui交互特征
3. TBD

# 一些经验：
- gpu加速lgbm训练速度约x30
- lgbm超参对于结果影响很小
- ranker对于无交互的负例直接全部过滤
- 内存不足用pandas分chunk处理

