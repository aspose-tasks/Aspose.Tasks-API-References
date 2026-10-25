---
title: "类 TaskBaseline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskBaseline 类。表示任务的基线。"
type: docs
weight: 2370
url: /zh/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

表示任务的基线。

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | 初始化 `TaskBaseline` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | 获取或设置基线数据记录的唯一编号。 |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | 获取或设置资源在项目截至目前执行的工作的预算成本。 |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | 获取或设置为资源计划的工作的预算成本。 |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | 获取或设置基线保存时资源的预计成本。 |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | 获取或设置基线保存时任务的计划持续时间。 |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | 获取或设置一个值，指示任务的基线持续时间是否为估计值。 |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | 获取或设置基线保存时任务的计划完成日期。 |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | 获取或设置基线保存时任务的固定成本。 |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | 获取或设置一个值，指示这是否是临时基线。 |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | 获取或设置基线保存时任务的计划开始日期。 |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | 获取或设置此对象的 TimephasedDataCollection 实例。与任务基线关联的时间分段数据。 |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | 获取或设置基线保存时分配给资源的工作量。基线保存时分配给资源的工作量。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。 |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。 |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | 返回一个值，指示此实例是否等于指定的 TaskBaseline 对象。 |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | 返回 `TaskBaseline` 类实例的哈希码值。 |

## 示例

展示如何获取基线信息。

```csharp
var project = new Project();

// 创建 TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 显示任务基线持续时间
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// 指示这是否是临时基线的值
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// 打印任务基线的时间分段数据
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### 另见

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


