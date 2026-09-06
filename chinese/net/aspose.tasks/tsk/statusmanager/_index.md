---
title: "Tsk.StatusManager"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。接收来自资源的当前任务状态更新的企业资源名称"
type: docs
weight: 1050
url: /zh/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

企业资源的名称，该资源将从资源处接收当前任务的状态更新。

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## 示例

展示如何读取/写入 Tsk.StatusManager 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


