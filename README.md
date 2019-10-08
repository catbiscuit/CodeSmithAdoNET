# CodeSmithAdoNET
ADONET三层结构

2019-10-08
1.Model.cst写的不完善，对字段类型not null没有进行判断，目前全是可空类型。
（1）示例
CreateDate DateTime not null，
生成的字段为 public DateTime？ CreateDate {get;set;}
正确的字段为 public DateTime CreateDate {get;set;}
