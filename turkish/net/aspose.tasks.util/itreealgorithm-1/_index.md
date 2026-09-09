---
title: "Arayüz ITreeAlgorithmT"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.ITreeAlgorithm1T arayüzü. T nesnelerinden oluşan bir ağaç üzerine uygulanabilen bir algoritmayı temsil eder."
type: docs
weight: 2730
url: /tr/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

*T* nesnelerinin bir ağacına uygulanabilen bir algoritmayı temsil eder.

```csharp
public interface ITreeAlgorithm<in T>
```

| Parametre | Açıklama |
| --- | --- |
| T | Yöntem arayüzünün uygulanacağı nesnenin türü. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | Bir ağacın düğümünü işler. |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | Bir ağacın düğümünün işlenmesinden sonra çağrılır. |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | Bir ağacın düğümünün işlenmesinden önce çağrılır. |

## Örnekler

&lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt; ağaç tabanlı algoritmanın nasıl kullanılacağını gösterir.

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

    // ağaç algoritmasını ortak işi toplamak ve işi güncellemek için kullan
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary><see cref=\"WorkAccumulator\" /> sınıfının yeni bir örneğini başlatır.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // ön algoritma adımlarında yapılacak bir şey yok
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
        // son algoritma adımlarında yapılacak bir şey yok
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


