---
title: "Rsc.PeakUnits"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源在任意时刻对其被分配的所有任务的最大分配单位"
type: docs
weight: 540
url: /zh/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

资源在任何时刻对其分配的所有任务的最大分配单位。

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## 示例

展示如何读取/写入 Rsc.PeakUnits 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


