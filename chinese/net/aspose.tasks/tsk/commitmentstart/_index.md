---
title: "Tsk.CommitmentStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。交付的开始日期。仅支持 XML 格式的读取。"
type: docs
weight: 180
url: /zh/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

交付的开始日期。仅支持 XML 格式的读取。

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## 示例

展示如何读取/写入 Tsk.CommitmentStart 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


