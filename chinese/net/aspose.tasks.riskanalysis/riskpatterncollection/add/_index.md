---
title: "RiskPatternCollection.Add"
second_title: "Aspose.Tasks for .NET API 参考"
description: "RiskPatternCollection 方法。向此集合添加一个 RiskPattern 类的实例。"
type: docs
weight: 40
url: /zh/net/aspose.tasks.riskanalysis/riskpatterncollection/add/
---
## RiskPatternCollection.Add method

向此集合添加一个 [`RiskPattern`](../../riskpattern/) 类的实例。

```csharp
public void Add(RiskPattern item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | RiskPattern | 要添加到此集合的 [`RiskPattern`](../../riskpattern/) 类的实例。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *item* 任务为 null。 |

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

* class [RiskPattern](../../riskpattern/)
* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


