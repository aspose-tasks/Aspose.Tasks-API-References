---
title: "ITreeAlgorithm1.PostAlg"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ITreeAlgorithm. Appelée après le traitement d'un nœud d'un arbre"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/itreealgorithm-1/postalg/
---
## ITreeAlgorithm&lt;T&gt;.PostAlg method

Appelé après le traitement d'un nœud d'un arbre.

```csharp
public void PostAlg(T el, int level)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | Nœud à traiter. |
| niveau | Int32 | Niveau du nœud d'arbre. |

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

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


