题目：校园一卡通管理系统

功能要求：
1. 卡管理：开户、挂失、补卡、销户、存钱、查询等。
2. 图书借阅：借书、续借、还书、查询等。
3. 消费：各类刷卡消费，如食堂、仓买、洗浴、健身、查询统计等。
4. 门禁：开通、禁止、查询等控制功能。
5. 签到：刷卡签到、统计等功能。

系统架构：
由东、西、南三个校区的数据库构成，每校区有一个数据库。一卡通的注册、销户等只能在西区数据库内完成，只有西区数据库有学生卡的table，其他数据库可以有消费、门禁、签到等相应功能的table，但卡的数据只能到西区数据库读，需要建立数据库链接。

完成目标：
1. 创建数据库，三个校区每区一个,west, east, south；
2. 创建表空间，userdata；
3. 创建表，根据以上需求描述创建表及约束、索引、视图；
4. 创建用户，卡管理员、图书管理员、门禁管理员、售货员、学生、教师等，不同人员有不同的数据库访问权限。
5. 开发相应的数据库端程序，如触发器、存储过程、函数等。
6. 开发前台界面，可以简化，不必考虑美观，语言不限。Java, c++, c#等均可。
