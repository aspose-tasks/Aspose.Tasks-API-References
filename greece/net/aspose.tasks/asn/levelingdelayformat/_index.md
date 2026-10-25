---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η μορφή διάρκειας μιας καθυστέρησης."
type: docs
weight: 320
url: /el/net/aspose.tasks/asn/levelingdelayformat/
---
## Asn.LevelingDelayFormat field

Η μορφή διάρκειας μιας καθυστέρησης.

```csharp
public static readonly Key<TimeUnitType, AsnKey> LevelingDelayFormat;
```

### Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες Asn.Delay, Asn.LevelingDelay και Asn.LevelingDelayFormat.

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
Console.WriteLine("Leveling Delay Format: " + assignment.Get(Asn.LevelingDelayFormat));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
