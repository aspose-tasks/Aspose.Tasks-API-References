---
title: "Tsk.FixedCostAccrual"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Καθορίζει επιλογές για το πώς και πότε τα σταθερά κόστη πρέπει να χρεωθούν ή να καταγραφούν στο κόστος μιας εργασίας."
type: docs
weight: 440
url: /el/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Καθορίζει επιλογές για το πώς και πότε τα σταθερά κόστη χρεώνονται ή συσσωρεύονται στο κόστος μιας εργασίας.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


