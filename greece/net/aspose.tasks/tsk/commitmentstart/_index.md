---
title: "Tsk.CommitmentStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ημερομηνία έναρξης μιας παράδοσης. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML."
type: docs
weight: 180
url: /el/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

Η ημερομηνία έναρξης μιας παράδοσης. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


