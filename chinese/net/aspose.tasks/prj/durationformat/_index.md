---
title: "Prj.DurationFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。用于表示总体持续时间的格式"
type: docs
weight: 300
url: /zh/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

表示批量持续时间的格式。

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## 示例

展示如何读取/写入 Prj.DurationFormat 属性。

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


