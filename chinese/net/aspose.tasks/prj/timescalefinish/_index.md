---
title: "Prj.TimescaleFinish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。视图中时间尺度的结束日期。"
type: docs
weight: 730
url: /zh/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

视图中时间尺度结束的日期。

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## 示例

展示如何读取/写入 Prj.TimescaleFinish 属性。

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


