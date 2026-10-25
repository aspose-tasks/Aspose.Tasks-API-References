---
title: "Rsc.Work"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。为资源在任务上安排的总时间"
type: docs
weight: 690
url: /zh/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

资源在任务上计划的总时间。

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## 示例

展示如何读取/写入 Rsc.Work 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


