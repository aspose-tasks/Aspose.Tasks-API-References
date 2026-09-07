---
title: "Tsk.BudgetWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Pekerjaan anggaran untuk sumber daya anggaran dan material. Sumber daya anggaran hanya ditugaskan ke tugas ringkasan proyek"
type: docs
weight: 150
url: /id/net/aspose.tasks/tsk/budgetwork/
---
## Tsk.BudgetWork field

Pekerjaan anggaran untuk pekerjaan anggaran dan sumber daya material. Sumber daya anggaran hanya ditugaskan ke tugas ringkasan proyek.

```csharp
public static readonly Key<Duration, TaskKey> BudgetWork;
```

## Contoh

Menampilkan cara membaca nilai pekerjaan/biaya anggaran dari tugas/sumber daya/penugasan.

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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


