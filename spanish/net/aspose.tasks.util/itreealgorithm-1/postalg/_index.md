---
title: "ITreeAlgorithm1.PostAlg"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ITreeAlgorithm. Se llama después del procesamiento de un nodo de un árbol"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/itreealgorithm-1/postalg/
---
## ITreeAlgorithm&lt;T&gt;.PostAlg method

Llamado después del procesamiento de un nodo de un árbol.

```csharp
public void PostAlg(T el, int level)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
| nivel | Int32 | Nivel del nodo del árbol. |

## Ejemplos

Muestra cómo usar el algoritmo basado en árbol &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt;.

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

    // utiliza el algoritmo de árbol para recopilar trabajo común y actualizar el trabajo
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Inicializa una nueva instancia de la clase <see cref=\"WorkAccumulator\" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // no hay nada que hacer en los pasos previos del algoritmo
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
        // no hay nada que hacer en los pasos posteriores del algoritmo
    }
}
```

### Ver también

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


