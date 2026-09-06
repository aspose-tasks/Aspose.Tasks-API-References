---
title: "TaskBaseline.FixedCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskBaseline 属性。获取或设置基线保存时任务的固定成本"
type: docs
weight: 50
url: /zh/net/aspose.tasks/taskbaseline/fixedcost/
---
## TaskBaseline.FixedCost property

获取或设置基线保存时任务的固定成本。

```csharp
public double FixedCost { get; set; }
```

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

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


