---
title: "Tsk.IsMarked"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。显示任务是否已标记以进行进一步操作或某种标识。"
type: docs
weight: 620
url: /zh/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

显示任务是否被标记为需要进一步操作或某种标识。

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## 备注

仅适用于 mpp 文件格式。

## 示例

展示如何读取/写入 Tsk.IsMarked 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


