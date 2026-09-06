---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。实际加班工作受保护的工作量"
type: docs
weight: 60
url: /zh/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

实际加班工作受保护的工作量。

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## 示例

展示如何读取/写入 Rsc.ActualOvertimeWorkProtected 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


