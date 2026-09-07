---
title: "ITreeAlgorithm1.PostAlg"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ITreeAlgorithm. Dipanggil setelah memproses sebuah node dari pohon"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/itreealgorithm-1/postalg/
---
## ITreeAlgorithm&lt;T&gt;.PostAlg method

Dipanggil setelah pemrosesan sebuah node pada pohon.

```csharp
public void PostAlg(T el, int level)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
| tingkat | Int32 | Level node pohon. |

## Contoh

Menampilkan cara menggunakan algoritma berbasis pohon &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt;.

```csharp
public void WorkWithITreeAlgorithm()
{
    var project = new Project(DataDir + "Project1.mpp");

    var root = project.RootTask.Children.Add("Project Management");
    var summary = root.Children.Add("Manage iteration");

    var task = summary.Children.Add("Acquire staff");
    task.Set(Tsk.Start, new DateTime(1999, 5, 3, 9, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(8 * 14, TimeUnitType.Hour));
    task.Set(Tsk.Finish, project.Get(Prj.Calendar).GetFinishDateByStartAndWork(task.Get(Tsk.Start), task.Get(Tsk.Duration)));

    var resource = project.Resources.Add("Project Manager");
    resource.Set(Rsc.Type, ResourceType.Work);

    project.ResourceAssignments.Add(task, resource);

    // gunakan algoritma pohon untuk mengumpulkan pekerjaan umum dan memperbarui pekerjaan
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Menginisialisasi instance baru dari kelas <see cref=\"WorkAccumulator\" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // tidak ada yang harus dilakukan pada langkah pra-algoritma
    }

    public void Alg(Task el, int level)
    {
        if (!el.Get(Tsk.IsSummary))
        {
            this.Work.Add(el.Get(Tsk.Work));
        }
    }

    public void PostAlg(Task el, int level)
    {
        // tidak ada yang harus dilakukan pada langkah pasca-algoritma
    }
}
```

### Lihat Juga

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


