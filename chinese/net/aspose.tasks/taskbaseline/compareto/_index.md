---
title: "TaskBaseline.CompareTo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskBaseline 方法。IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较"
type: docs
weight: 90
url: /zh/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。

```csharp
public int CompareTo(TaskBaseline other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | TaskBaseline | 用于与此实例比较的指定 Baseline 对象。 |

### 返回值

如果此实例小于指定对象则返回 -1，若大于指定对象则返回 1；否则返回 0。

## 示例

展示如何检查基线的相等性。

```csharp
var project = new Project();

// 创建 TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 显示任务基线持续时间
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// 基线的相等性是根据基线的数字进行检查的。
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### 另见

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


