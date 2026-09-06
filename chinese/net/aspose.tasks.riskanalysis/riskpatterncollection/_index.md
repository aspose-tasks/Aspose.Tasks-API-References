---
title: "类 RiskPatternCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RiskAnalysis.RiskPatternCollection 类。表示一个包含 RiskPattern 类实例的集合。"
type: docs
weight: 1940
url: /zh/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

表示一个包含 [`RiskPattern`](../riskpattern/) 类实例的集合。

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | 获取指定任务的 [`RiskPattern`](../riskpattern/) 类实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | 向此集合添加一个 [`RiskPattern`](../riskpattern/) 类的实例。 |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | 从此集合中移除特定对象的第一次出现。 |

## 示例

展示如何使用风险模式集合。

```csharp
var settings = new RiskAnalysisSettings
{
    // 设置 Monte Carlo 仿真的迭代次数（默认值为 100）。
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// 只要 RiskPatternCollection 不是只读的
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// 可以添加新模式
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// 遍历已添加的模式
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// 通过索引访问编辑集合中的模式
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// 编辑后检查模式
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// 我们可以移除该模式
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// 检查该模式不在集合中
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// 可以通过两种方式清除集合

// 将模式复制到数组中并逐个删除
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// 或者可以完全清空模式集合
settings.Patterns.Clear();
```

### 另见

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


