---
title: "Tsk.LevelingCanSplit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定资源平衡功能是否会在此任务的剩余工作上产生拆分"
type: docs
weight: 760
url: /zh/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

确定资源平衡功能是否会对该任务的剩余工作进行拆分。

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## 示例

展示如何读取/写入 Tsk.LevelingCanSplit 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


