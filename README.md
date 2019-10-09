# CodeSmithAdoNET
ADONET三层结构<br>
<br>
2019-10-08<br>
1.Model.cst写的不完善，对字段类型not null没有进行判断，目前全是可空类型。<br>
（1）示例<br>
CreateDate DateTime not null，<br>
生成的字段为 public DateTime？ CreateDate {get;set;}<br>
正确的字段为 public DateTime CreateDate {get;set;}<br>
