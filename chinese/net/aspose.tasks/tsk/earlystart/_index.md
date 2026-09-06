---
title: "Tsk.EarlyStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务可能开始的最早日期，基于前置任务和后续任务的最早开始日期以及其他约束。"
type: docs
weight: 340
url: /zh/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

基于前置和后续任务的最早开始日期以及其他约束，任务可能开始的最早日期。

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## 示例

展示如何读取/写入 Tsk.EarlyStart 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


