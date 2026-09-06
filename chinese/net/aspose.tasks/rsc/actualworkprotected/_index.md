---
title: "Rsc.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。实际工作受到保护的工作量"
type: docs
weight: 80
url: /zh/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

实际工作受保护的工作量。

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## 示例

展示如何读取/写入 Rsc.ActualWorkProtected 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


