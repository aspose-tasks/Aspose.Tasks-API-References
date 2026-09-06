---
title: "Tsk.StartText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。返回任务的开始文本"
type: docs
weight: 1030
url: /zh/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

返回任务的开始文本。

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## 示例

展示如何读取/写入 Tsk.StartText 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


