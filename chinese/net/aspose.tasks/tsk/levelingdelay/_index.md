---
title: "Tsk.LevelingDelay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。由于资源平衡，任务从其最早开始日期需要延迟的时间"
type: docs
weight: 770
url: /zh/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

由于资源平衡，任务相对于其最早开始日期的延迟时间。

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## 示例

展示如何读取/写入 Tsk.LevelingDelay 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


