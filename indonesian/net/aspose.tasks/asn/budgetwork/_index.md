---
title: "Asn.BudgetWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Asn field. Jumlah pekerjaan yang dianggarkan untuk sumber daya kerja atau material pada penugasan"
type: docs
weight: 160
url: /id/net/aspose.tasks/asn/budgetwork/
---
## Asn.BudgetWork field

Jumlah pekerjaan yang dianggarkan untuk pekerjaan atau sumber daya material pada penugasan.

```csharp
public static readonly Key<Duration, AsnKey> BudgetWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


