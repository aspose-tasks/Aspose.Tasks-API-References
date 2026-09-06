---
title: "TaskBaseline.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskBaseline 方法。返回一个值，指示此实例是否等于指定的 TaskBaseline 对象"
type: docs
weight: 100
url: /zh/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

返回一个值，指示此实例是否等于指定的 TaskBaseline 对象。

```csharp
public bool Equals(TaskBaseline other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | TaskBaseline | 用于与此实例比较的指定 AssignmentBaseline 对象。 |

### 返回值

如果此实例等于指定的 TaskBaseline 对象则返回 true；否则返回 false。

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

---

## Equals(object) {#equals_2}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 与此实例比较的对象。 |

### 返回值

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


