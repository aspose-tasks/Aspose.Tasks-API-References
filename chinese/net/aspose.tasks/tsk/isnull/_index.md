---
title: "Tsk.IsNull"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否为空任务"
type: docs
weight: 640
url: /zh/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

确定任务是否为空任务。

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## 示例

展示如何读取/写入 Tsk.IsNull 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


