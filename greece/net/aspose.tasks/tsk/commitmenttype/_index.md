---
title: "Tsk.CommitmentType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία έχει μια συσχετισμένη παράδοση ή μια εξάρτηση από μια συσχετισμένη παράδοση. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML."
type: docs
weight: 190
url: /el/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Καθορίζει εάν ένα έργο έχει μια σχετική παράδοση ή μια εξάρτηση από μια σχετική παράδοση. Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


