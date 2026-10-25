---
title: "Rsc.RegularWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。计划由资源执行的非加班工作总量"
type: docs
weight: 570
url: /zh/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

资源计划执行的非加班工作总量。

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## 示例

展示如何读取/写入 Rsc.RegularWork 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


