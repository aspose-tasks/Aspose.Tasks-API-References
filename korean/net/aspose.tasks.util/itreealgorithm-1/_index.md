---
title: "인터페이스 ITreeAlgorithmT"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.ITreeAlgorithm1T 인터페이스. T 객체 트리에 적용할 수 있는 알고리즘을 나타냅니다."
type: docs
weight: 2730
url: /ko/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

*T* 객체 트리에 적용할 수 있는 알고리즘을 나타냅니다.

```csharp
public interface ITreeAlgorithm<in T>
```

| 매개변수 | 설명 |
| --- | --- |
| T | 메서드 인터페이스를 적용할 객체 유형. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | 트리의 노드를 처리합니다. |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | 트리 노드 처리 후에 호출됩니다. |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | 트리 노드 처리 전에 호출됩니다. |

## 예제

&lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt; 트리 기반 알고리즘 사용 방법을 보여줍니다.

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

    // 공통 작업을 수집하고 작업을 업데이트하기 위해 트리 알고리즘을 사용합니다.
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary><see cref=\"WorkAccumulator\" /> 클래스의 새 인스턴스를 초기화합니다.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // 알고리즘 사전 단계에서 할 일이 없습니다.
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
        // 알고리즘 사후 단계에서 할 일이 없습니다.
    }
}
```

### 또 보기

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


