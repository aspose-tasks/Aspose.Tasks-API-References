---
title: "Prj.CurrentDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。系统日期"
type: docs
weight: 190
url: /zh/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

系统日期。

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## 示例

展示如何读取/写入 Prj.CurrentDate 属性。

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


