---
title: "Rsc.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。已分配给任务的资源实际完成的加班工作量"
type: docs
weight: 50
url: /zh/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

已由分配到任务的资源实际完成的加班工作量。

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## 示例

展示如何读取/写入 Rsc.ActualOvertimeWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


