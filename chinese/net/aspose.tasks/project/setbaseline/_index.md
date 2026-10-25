---
title: "Project.SetBaseline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。将基线字段保存到整个项目的指定基线"
type: docs
weight: 1250
url: /zh/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

将基线字段保存到整个项目的指定基线。

```csharp
public void SetBaseline(BaselineType baselineType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baselineType | BaselineType | 用于保存基线数据的基线类型。 |

## 示例

展示如何为整个项目创建基线。

```csharp
var project = new Project();

// 添加任务
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// 为指定任务设置基线
project.SetBaseline(BaselineType.Baseline);
```

### 另见

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

将基线字段保存到所选任务的指定基线。

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baselineType | BaselineType | 用于保存基线数据的基线类型。 |
| taskCollection | IEnumerable`1 | 要保存基线数据的任务列表。 |

## 示例

展示如何为特定任务创建并设置基线。

```csharp
var project = new Project();

// 添加任务
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// 为指定任务设置基线
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### 另见

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


