---
title: "Rsc.Finish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段. 资源计划完成所有已分配任务工作的日期."
type: docs
weight: 290
url: /zh/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

资源计划完成所有分配任务工作的日期。

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## 示例

展示如何读取/写入 Rsc.Finish 属性.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


