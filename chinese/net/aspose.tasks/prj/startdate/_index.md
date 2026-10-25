---
title: "Prj.StartDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的开始日期"
type: docs
weight: 680
url: /zh/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

项目的开始日期。

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## 示例

展示如何读取/写入 Prj.StartDate 属性。

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


