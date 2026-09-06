---
title: "Tsk.DisplayAsSummary"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否应显示为汇总任务。仅支持 XML 格式的读取"
type: docs
weight: 280
url: /zh/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

确定任务是否应显示为汇总任务。仅支持 XML 格式的读取。

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## 示例

展示如何读取/写入 Tsk.DisplayAsSummary 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


