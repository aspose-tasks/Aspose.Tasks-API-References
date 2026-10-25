---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η μορφή έκφρασης της διάρκειας μιας καθυστέρησης."
type: docs
weight: 790
url: /el/net/aspose.tasks/tsk/levelingdelayformat/
---
## Tsk.LevelingDelayFormat field

Η μορφή έκφρασης της διάρκειας μιας καθυστέρησης.

```csharp
public static readonly Key<TimeUnitType, TaskKey> LevelingDelayFormat;
```

### Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.LevelingDelayFormat.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelayFormat, TimeUnitType.Hour);

Console.WriteLine("Leveling Delay Format: " + task.Get(Tsk.LevelingDelayFormat));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [TaskKey](../../taskkey)
* class [Tsk](../../tsk)
* namespace [Aspose.Tasks](../../tsk)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
