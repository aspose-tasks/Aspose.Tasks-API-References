---
title: "Tsk.Duration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Η συνολική διάρκεια ενεργού χρόνου εργασίας για μια εργασία όπως εισάγεται ή όπως υπολογίζεται από το Microsoft Project βάσει ημερομηνίας έναρξης, ημερομηνίας λήξης, ημερολογίων και άλλων παραγόντων προγραμματισμού."
type: docs
weight: 300
url: /el/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

Η συνολική διάρκεια του ενεργού χρόνου εργασίας για μια εργασία, όπως εισάγεται ή υπολογίζεται από το Microsoft Project με βάση την ημερομηνία έναρξης, την ημερομηνία λήξης, τα ημερολόγια και άλλους παράγοντες προγραμματισμού.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Παραδείγματα

Δείχνει πώς να ορίσετε τη διάρκεια της εργασίας.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


