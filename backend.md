# 用户添加关注分类

数据库格式：
f_id(INT unique), f_user_id(INT), f_category(INT 1-16种分类), f_ctime
f_user_id 1比1对应关系到 f_category

限制一个用户最多可以关注三个分类

## 如何在put接口里插入关注信息，且在更新关注的时候最优减少数据库操作次数？

put 接口接受数据 f_category = [1,13,16], f_user_id = 133
