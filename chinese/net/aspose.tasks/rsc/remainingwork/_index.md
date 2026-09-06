---
title: "Rsc.RemainingWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。完成任务或任务集仍需的时间"
type: docs
weight: 610
url: /zh/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

完成任务或任务集仍需的时间。

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## 示例

展示如何读取/写入 Rsc.RemainingWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


