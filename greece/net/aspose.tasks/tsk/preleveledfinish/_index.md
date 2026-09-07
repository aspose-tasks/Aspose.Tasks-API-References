---
title: "Tsk.PreleveledFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Η ημερομηνία λήξης μιας εργασίας όπως ήταν πριν γίνει εξισορρόπηση πόρων"
type: docs
weight: 910
url: /el/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

Η ημερομηνία λήξης μιας εργασίας όπως ήταν πριν γίνει η εξισορρόπηση πόρων.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


