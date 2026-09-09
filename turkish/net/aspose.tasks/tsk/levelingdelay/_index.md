---
title: "Tsk.LevelingDelay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynak dengelemesi nedeniyle bir görevin erken başlangıç tarihinden gecikmesi gereken süre"
type: docs
weight: 770
url: /tr/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

Kaynak dengelemesi nedeniyle bir görevin erken başlangıç tarihinden gecikmesi gereken süre.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Örnekler

Tsk.LevelingDelay özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


