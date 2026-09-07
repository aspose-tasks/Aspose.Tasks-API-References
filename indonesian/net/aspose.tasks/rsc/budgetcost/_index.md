---
title: "Rsc.BudgetCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Biaya anggaran untuk sumber daya biaya anggaran. Sumber daya anggaran hanya ditetapkan ke tugas ringkasan proyek"
type: docs
weight: 170
url: /id/net/aspose.tasks/rsc/budgetcost/
---
## Rsc.BudgetCost field

Biaya anggaran untuk sumber daya biaya anggaran. Sumber daya anggaran hanya ditugaskan ke tugas rangkuman proyek.

```csharp
public static readonly Key<decimal, RscKey> BudgetCost;
```

## Contoh

Menampilkan cara membaca nilai pekerjaan/biaya anggaran dari sebuah sumber daya.

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
foreach (var task in collector.Tasks)
{
    // Tampilkan pekerjaan anggaran penugasan dan biaya anggaran
    foreach (var assignment in task.Assignments)
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
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


