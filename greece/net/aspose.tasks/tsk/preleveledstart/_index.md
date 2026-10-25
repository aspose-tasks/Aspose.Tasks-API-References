---
title: "Tsk.PreleveledStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ημερομηνία έναρξης μιας εργασίας όπως ήταν πριν γίνει εξισορρόπηση πόρων"
type: docs
weight: 920
url: /el/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

Η ημερομηνία έναρξης μιας εργασίας όπως ήταν πριν γίνει η εξισορρόπηση πόρων.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


