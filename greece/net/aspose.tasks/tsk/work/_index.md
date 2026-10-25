---
title: "Tsk.Work"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ο συνολικός χρόνος που έχει προγραμματιστεί για μια εργασία για όλους τους εκχωρημένους πόρους"
type: docs
weight: 1150
url: /el/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

Ο συνολικός προγραμματισμένος χρόνος σε μια εργασία για όλους τους ανατεθειμένους πόρους.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


