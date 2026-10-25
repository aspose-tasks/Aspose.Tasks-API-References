---
title: "Prj.DefaultFinishTime"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。新任务的默认完成时间"
type: docs
weight: 230
url: /zh/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

新任务的默认完成时间。

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## 示例

展示如何读取/写入 Prj.DefaultFinishTime 属性。

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


