---
title: "Tsk.LevelingDelay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Ο χρόνος που μια εργασία πρέπει να καθυστερήσει από την αρχική ημερομηνία έναρξής της λόγω εξισορρόπησης πόρων"
type: docs
weight: 770
url: /el/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

Ο χρόνος που μια εργασία πρέπει να καθυστερήσει από την αρχική ημερομηνία έναρξής της λόγω εξισορρόπησης πόρων.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


