---
title: "TaskBaseline.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskBaseline 方法。返回 TaskBaseline 类实例的哈希码值"
type: docs
weight: 110
url: /zh/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

返回 [`TaskBaseline`](../) 类实例的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取任务基线的哈希码。

```csharp
var project = new Project();

// 创建 TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 显示任务基线持续时间
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// 日历的哈希码等于基线编号
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### 另见

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


