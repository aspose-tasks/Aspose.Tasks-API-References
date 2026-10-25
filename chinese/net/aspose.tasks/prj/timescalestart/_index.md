---
title: "Prj.TimescaleStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。视图中时间尺度的开始日期。"
type: docs
weight: 740
url: /zh/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

视图中时间尺度开始的日期。

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## 示例

展示如何设置时间尺度开始日期，以调整视图应开始的日期。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


