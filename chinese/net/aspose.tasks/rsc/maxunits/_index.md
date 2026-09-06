---
title: "Rsc.MaxUnits"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源在当前时间段内可用于完成任何任务的最大容量所对应的最大单元数"
type: docs
weight: 450
url: /zh/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

表示资源在当前时间段内可用于完成任何任务的最大容量的最大单位数。

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## 示例

展示如何读取/写入 Rsc.MaxUnits 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


