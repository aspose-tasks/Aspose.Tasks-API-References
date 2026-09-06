---
title: "Tsk.DisplayOnTimeline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。指定任务是否应显示在时间线视图中"
type: docs
weight: 290
url: /zh/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

指定任务是否应在时间轴视图中显示。

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## 示例

展示如何读取/写入 Tsk.DisplayOnTimeline 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


