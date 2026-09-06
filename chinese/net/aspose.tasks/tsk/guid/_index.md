---
title: "Tsk.Guid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 为任务生成的唯一标识代码."
type: docs
weight: 460
url: /zh/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

为任务生成的唯一标识代码。

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## 示例

展示如何读取/写入 Tsk.Guid 属性.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


