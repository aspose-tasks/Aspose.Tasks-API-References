---
title: "接口 ITreeAlgorithmT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.ITreeAlgorithm1T 接口。表示一种可应用于对象 T 树的算法"
type: docs
weight: 2730
url: /zh/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

表示可应用于对象树 *T* 的算法。

```csharp
public interface ITreeAlgorithm<in T>
```

| 参数 | 描述 |
| --- | --- |
| T | 要将方法接口应用于的对象类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | 处理树的节点。 |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | 在处理树的节点之后调用。 |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | 在处理树的节点之前调用。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt; 基于树的算法。

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

    // 使用树算法收集通用工作并更新工作
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>初始化 <see cref=\"WorkAccumulator\" /> 类的新实例。</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // 在算法前置步骤中没有要执行的操作
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
        // 在算法后置步骤中没有要执行的操作
    }
}
```

### 另见

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


