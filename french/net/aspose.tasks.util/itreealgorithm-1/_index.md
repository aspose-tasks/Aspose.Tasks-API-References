---
title: "Interface ITreeAlgorithmT"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Util.ITreeAlgorithm1T interface. Représente un algorithme qui peut être appliqué à un arbre d'objets T"
type: docs
weight: 2730
url: /fr/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

Représente un algorithme qui peut être appliqué à un arbre d'objets *T*.

```csharp
public interface ITreeAlgorithm<in T>
```

| Paramètre | Description |
| --- | --- |
| T | Le type d'objet auquel appliquer l'interface de méthode. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | Traite un nœud d'un arbre. |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | Appelé après le traitement d'un nœud d'un arbre. |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | Appelé avant le traitement d'un nœud d'un arbre. |

## Exemples

Montre comment utiliser l'algorithme basé sur l'arbre &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt;.

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

    // utilisez l'algorithme d'arbre pour rassembler le travail commun et mettre à jour le travail
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Initialise une nouvelle instance de la classe <see cref=\"WorkAccumulator\" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // il n'y a rien à faire dans les étapes pré-algorithme
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
        // il n'y a rien à faire dans les étapes post-algorithme
    }
}
```

### Voir aussi

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


