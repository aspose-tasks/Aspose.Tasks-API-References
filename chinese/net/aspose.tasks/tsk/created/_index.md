---
title: "Tsk.Created"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务创建的日期"
type: docs
weight: 250
url: /zh/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

任务创建的日期。

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## 示例

展示如何读取/写入 Tsk.Created 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


