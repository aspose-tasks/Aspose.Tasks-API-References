---
title: "Asn.BudgetCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Biaya anggaran sumber daya pada sebuah penugasan."
type: docs
weight: 150
url: /id/net/aspose.tasks/asn/budgetcost/
---
## Asn.BudgetCost field

Biaya yang dianggarkan untuk sumber daya pada penugasan.

```csharp
public static readonly Key<decimal, AsnKey> BudgetCost;
```

## Contoh

Menampilkan cara membaca nilai pekerjaan/biaya anggaran dari penugasan sumber daya.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// Tampilkan pekerjaan anggaran dan biaya anggaran untuk tugas ringkasan proyek
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// Tampilkan pekerjaan anggaran sumber daya
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// Tampilkan biaya anggaran sumber daya
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var tsk in collector.Tasks)
{
    // Tampilkan pekerjaan anggaran penugasan dan biaya anggaran
    foreach (var assignment in tsk.Assignments)
    {
        var resource = assignment.Get(Asn.Resource);
        if (resource == null)
        {
            continue;
        }

        if (resource.Get(Rsc.Type) == ResourceType.Work)
        {
            Console.WriteLine("Assignment BudgetWork = " + assignment.Get(Asn.BudgetWork));
        }
        else
        {
            Console.WriteLine("Assignment BudgetCost = " + assignment.Get(Asn.BudgetCost));
        }
    }
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


