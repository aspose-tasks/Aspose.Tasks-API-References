---
title: "类 TaskBaselineCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskBaselineCollection 类。表示 TaskBaseline 对象的集合。"
type: docs
weight: 2380
url: /zh/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

表示一个 [`TaskBaseline`](../taskbaseline/) 对象的集合。

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | 获取此 TaskBaselineCollection 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | 返回指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。 |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | 从此集合中移除基线。 |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | 将 TaskBaselineCollection 对象转换为 [`TaskBaseline`](../taskbaseline/) 对象的列表。 |

## 示例

展示如何使用任务基线集合。

```csharp
var project = new Project();

// 创建项目基线
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 打印任务基线
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// 清除所有基线
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### 另见

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


