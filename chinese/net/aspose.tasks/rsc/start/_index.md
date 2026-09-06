---
title: "Rsc.Start"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。已分配资源计划开始在任务上工作的日期"
type: docs
weight: 640
url: /zh/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

已分配资源计划开始在任务上工作的日期。

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## 示例

展示如何读取/写入 Rsc.Start 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


