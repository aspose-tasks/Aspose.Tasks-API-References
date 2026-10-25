---
title: "Project.Recalculate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。重新安排所有项目任务的 ID、大纲层级、开始/结束日期，设置提前/延后日期，计算时差、工作量和成本字段。"
type: docs
weight: 1150
url: /zh/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

重新安排所有项目任务的 ID、大纲级别、开始/完成日期，设置提前/延后日期，计算浮动、工作和成本字段。

```csharp
public void Recalculate()
```

## 示例

展示如何从开始日期而不是结束日期重新安排项目。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// 现在所有任务日期（Start、Finish、EarlyStart、EarlyFinish、LateStart、LateFinish）已计算。要获取关键路径，我们需要计算时差（可以在单独线程中调用，但必须在所有早/晚日期计算完成后）。
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

重新安排所有项目任务的 ID、大纲级别、开始/完成日期，设置提前/延后日期，计算浮动、工作和成本字段（可选验证）。

```csharp
public void Recalculate(bool validate)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| validate | Boolean | 如果为 true，将执行重新计算的验证。验证哪些数据：目前仅实现对任务及任务链接日期范围的基本验证。任务的日期范围（例如 ActualStart - ActualFinish、EarlyStart - EarlyFinish 等）以及任务链接的日期将根据开始日期小于或等于结束日期的标准进行检查。如果上述任何条件未满足，则会抛出 [`RecalculationValidationException`](../../recalculationvalidationexception/)。 |

## 示例

展示如何在后置验证后重新计算项目。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // 在后置验证后重新计算项目
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


