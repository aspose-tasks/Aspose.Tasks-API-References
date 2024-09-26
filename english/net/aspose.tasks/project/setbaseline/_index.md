---
title: Project.SetBaseline
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Saves baseline fields to the specified baseline for the entire project
type: docs
weight: 1250
url: /net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Saves baseline fields to the specified baseline for the entire project.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | BaselineType | The baseline type to save baseline data to. |

## Examples

Shows how to create baselines for a whole project.

```csharp
var project = new Project();

// Adding tasks
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Set baseline for specified tasks
project.SetBaseline(BaselineType.Baseline);
```

### See Also

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Saves baseline fields to the specified baseline for the selected tasks.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | BaselineType | The baseline type to save baseline data to. |
| taskCollection | IEnumerable`1 | List of tasks to save baseline data for. |

## Examples

Shows how to create set baselines for specific tasks.

```csharp
var project = new Project();

// Adding tasks
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Set baseline for specified tasks
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### See Also

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


