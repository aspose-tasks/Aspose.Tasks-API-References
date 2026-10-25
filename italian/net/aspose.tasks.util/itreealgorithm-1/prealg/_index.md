---
title: "ITreeAlgorithm1.PreAlg"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ITreeAlgorithm. Chiamato prima dell'elaborazione di un nodo di un albero"
type: docs
weight: 30
url: /it/net/aspose.tasks.util/itreealgorithm-1/prealg/
---
## ITreeAlgorithm&lt;T&gt;.PreAlg method

Chiamato prima dell'elaborazione di un nodo di un albero.

```csharp
public void PreAlg(T el, int level)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | Nodo da elaborare. |
| livello | Int32 | Livello del nodo dell'albero. |

## Esempi

Mostra come utilizzare l'algoritmo basato su albero &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt;.

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

    // utilizza l'algoritmo ad albero per raccogliere il lavoro comune e aggiornare il lavoro
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Inizializza una nuova istanza della classe <see cref=\"WorkAccumulator\" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // non c'è nulla da fare nei passaggi pre-algoritmo
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
        // non c'è nulla da fare nei passaggi post-algoritmo
    }
}
```

### Vedi anche

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


