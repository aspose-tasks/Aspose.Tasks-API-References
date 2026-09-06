---
title: "Rsc.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。剩余已安排的加班时间量"
type: docs
weight: 600
url: /zh/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

剩余计划加班的数量。

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## 示例

展示如何读取/写入 Rsc.RemainingOvertimeWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


