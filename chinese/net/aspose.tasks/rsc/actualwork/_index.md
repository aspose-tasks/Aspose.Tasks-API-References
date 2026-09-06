---
title: "Rsc.ActualWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。已分配给任务的资源已完成的工作量"
type: docs
weight: 70
url: /zh/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

已由分配到任务的资源完成的工作量。

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## 示例

展示如何读取/写入 Rsc.ActualWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


