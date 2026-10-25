---
title: "Tsk.LateFinish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务可以完成的最晚日期，且不会延迟项目的完成时间"
type: docs
weight: 730
url: /zh/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

任务可以完成而不延迟项目完成的最晚日期。

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## 示例

展示如何读取/写入 Tsk.LateFinish 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


