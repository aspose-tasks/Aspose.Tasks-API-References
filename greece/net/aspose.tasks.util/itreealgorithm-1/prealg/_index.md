---
title: "ITreeAlgorithm1.PreAlg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ITreeAlgorithm. Καλείται πριν από την επεξεργασία ενός κόμβου δέντρου"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/itreealgorithm-1/prealg/
---
## ITreeAlgorithm&lt;T&gt;.PreAlg method

Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου.

```csharp
public void PreAlg(T el, int level)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | Int32 | Επίπεδο κόμβου δέντρου. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref="Aspose.Tasks.Util.ITreeAlgorithm`1" /&gt; αλγόριθμο βασισμένο σε δέντρο.

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

    // χρησιμοποιήστε αλγόριθμο δέντρου για να συγκεντρώσετε κοινή εργασία και να ενημερώσετε την εργασία
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Αρχικοποιεί μια νέα παρουσία της κλάσης <see cref="WorkAccumulator" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // Δεν υπάρχει τίποτα να κάνετε στα βήματα προ-αλγορίθμου
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
        // Δεν υπάρχει τίποτα να κάνετε στα βήματα μετα-αλγορίθμου
    }
}
```

### Δείτε επίσης

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


