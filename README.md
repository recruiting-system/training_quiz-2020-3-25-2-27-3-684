**需求描述**  
- 某数据平台，存储用户的信息
- 每个用户有id，参考编号，姓名，类型，地址，电话，邮箱数据信息。其中id、参考编号和电话只包含数字，类型只有'payer'、'buyer'和'deliverer' 
- 补全代码，实现管理者的要求

要求：
1. 根据需求描述建立合适的数据表，通过程序插入初始数据
2. 管理者可以一次性查找到所有的人物数据
3. 管理者可以通过单个id和姓名查找数据（可以单个条件查找，也可以联合查找），要求输入的id只包含数字，如果包含其他字符，则告诉管理者输入的id不符合要求
4. 管理者可以通过参考编号对查找出来的数据进行排序，正反排序的选择通过输入的参数决定
5. 查找到的数据全部转化为小写并去除掉数据前后的空格，在Application中通过json格式打印
6. 如果查找的数据不完整，其中有数据为空，则默认没有该条数据

延伸：  
满足上述要求的基础上
1. 管理者可以通过输入多个类型查找数据，输入的类型只能为'payer'、'buyer'和'deliverer'，如果输入了其他类型，则告诉管理者输入的类型不符合要求（管理者的输入为字符串）
2. 管理者可以通过电话号码对查找出来的数据排序，正反排序的选择通过管理者的输入决定