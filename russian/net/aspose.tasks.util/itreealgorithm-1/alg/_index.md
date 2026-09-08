---
title: "ITreeAlgorithm1.Alg"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ITreeAlgorithm. Обрабатывает узел дерева"
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/itreealgorithm-1/alg/
---
## ITreeAlgorithm&lt;T&gt;.Alg method

Обрабатывает узел дерева.

```csharp
public void Alg(T el, int level)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | T | Узел для обработки. |
| уровень | Int32 | Уровень узла дерева. |

## Примеры

Показывает, как использовать &lt;see cref="Aspose.Tasks.Util.ITreeAlgorithm`1" /&gt; алгоритм, основанный на дереве.

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

    // используйте алгоритм дерева для сбора общей работы и обновления работы 
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Инициализирует новый экземпляр класса <see cref="WorkAccumulator" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // нет ничего, что нужно сделать на предварительных шагах алгоритма
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
        // нет ничего, что нужно сделать на завершающих шагах алгоритма
    }
}
```

### См. также

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


