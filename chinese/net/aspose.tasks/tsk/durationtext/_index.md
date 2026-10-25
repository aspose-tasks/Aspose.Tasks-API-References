---
title: "Tsk.DurationText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。返回任务的持续时间文本"
type: docs
weight: 310
url: /zh/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

返回任务的持续时间文本。

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## 示例

展示如何读取/写入 Tsk.DurationText 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


