---
title: "Tsk.CommitmentFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ημερομηνία λήξης μιας παράδοσης. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML"
type: docs
weight: 170
url: /el/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

Η ημερομηνία λήξης μιας παράδοσης. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


