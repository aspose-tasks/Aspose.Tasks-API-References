---
title: "WorkingTime.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WorkingTime 方法。检查对象是否相等"
type: docs
weight: 40
url: /zh/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

检查对象是否相等。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 第二个要比较的对象。 |

### 返回值

如果对象相等则为 true，否则为 false。

## 示例

展示如何检查工作时间相等性。

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// 日历的相等性是根据工作时间的起始和结束日期进行检查的。
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### 另见

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


