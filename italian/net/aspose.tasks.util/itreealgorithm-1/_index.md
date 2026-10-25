---
title: "Interfaccia ITreeAlgorithmT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Interfaccia Aspose.Tasks.Util.ITreeAlgorithm1T. Rappresenta un algoritmo che può essere applicato a un albero di oggetti T"
type: docs
weight: 2730
url: /it/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

Rappresenta un algoritmo che può essere applicato a un albero di oggetti *T*.

```csharp
public interface ITreeAlgorithm<in T>
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'interfaccia del metodo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | Elabora un nodo di un albero. |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | Chiamato dopo l'elaborazione di un nodo di un albero. |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | Chiamato prima dell'elaborazione di un nodo di un albero. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


