---
title: "Tsk.IsExpanded"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定在 GanttChart 视图中汇总任务是否展开。"
type: docs
weight: 590
url: /zh/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

确定在甘特图视图中汇总任务是否展开。

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## 示例

展示如何读取/写入 Tsk.IsExpanded 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


