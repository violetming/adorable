此项目为uni-app

轮播图表

| 字段 | 类型    | 备注       |
| ---- | ------- | ---------- |
| id   | int     |            |
| 图片 | varchar | 图片存地址 |

图片就做三张图片的查询或者只放三张图片

宠物领养

| 字段 | 类型    | 备注                                               |
| ---- | ------- | -------------------------------------------------- |
| id   | int     |                                                    |
| 姓名 | varchar | 宠物姓名                                           |
| 图片 | varchar | 图片地址                                           |
| 类型 | varchar | 动物品种（边牧，狸花猫）或者考虑将品种单独做一个表 |
| 年龄 | int     |                                                    |
| 描述 | varchar | 领养的详情                                         |

问医生

| 字段     | 类型    | 备注           |
| -------- | ------- | -------------- |
| id       | int     |                |
| 图片     | varchar | 医生大头照     |
| 姓名     | varchar |                |
| 从业年限 | varchar |                |
| 擅长领域 | varchar | 擅长治疗什么病 |
| 个人简介 | varchar |                |
| 所在医院 | varchar | 关联医院（?）  |

推荐文章

| 字段 | 类型    | 备注                                     |
| ---- | ------- | ---------------------------------------- |
| id   | int     |                                          |
| 标题 | varchar |                                          |
| 内容 | varchar |                                          |
| 图片 | varchar |                                          |
| 喜欢 | int     | 点击之后想另一个表添加（想一下怎么做的） |
