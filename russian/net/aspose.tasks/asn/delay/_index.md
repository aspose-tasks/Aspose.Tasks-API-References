---
title: "Asn.Delay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Задержка назначения"
type: docs
weight: 230
url: /ru/net/aspose.tasks/asn/delay/
---
## Asn.Delay field

Задержка назначения.

```csharp
public static readonly Key<Duration, AsnKey> Delay;
```

## Примеры

Показывает, как читать/записывать свойства Asn.Delay и Asn.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


