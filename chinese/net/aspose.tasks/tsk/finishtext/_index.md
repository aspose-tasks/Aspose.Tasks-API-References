---
title: "Tsk.FinishText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。返回任务的完成文本"
type: docs
weight: 410
url: /zh/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

返回任务的完成文本。

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## 示例

展示如何读取/写入 Tsk.FinishText 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


