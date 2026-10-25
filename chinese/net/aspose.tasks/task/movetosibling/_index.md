---
title: "Task.MoveToSibling"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。将当前任务在相同的大纲级别上移动到指定任务之前。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate。它将重新安排所有项目任务的开始/结束日期，设置提前/延后日期，并计算诸如余量、工作和成本字段、大纲级别等依赖字段。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 ID、大纲级别和大纲编号。如果 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务的开始/结束日期，设置提前/延后日期，计算余量、工作和成本字段，重新计算 ID 和大纲级别。"
type: docs
weight: 1370
url: /zh/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

将当前任务在相同的 Outline Level 上移动到指定任务之前。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如时差、工作和成本字段、轮廓级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 id、轮廓级别和轮廓编号。若 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务（开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段，重新计算 id 和轮廓级别）。

```csharp
public void MoveToSibling(Task beforeTask)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| beforeTask | 任务 | 将在其之前插入当前任务的 Task。 |

## 示例

展示如何在相同的父级下移动任务。

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// 将 ID 为 5 的任务移动到 ID 为 3 的任务之前
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// 或
// 将任务移动到集合的末尾
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

将当前任务在相同的 Outline Level 上移动到具有指定 Id 的任务之前。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如时差、工作和成本字段、轮廓级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 id、轮廓级别和轮廓编号。若 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务（开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段，重新计算 id 和轮廓级别）。

```csharp
public void MoveToSibling(int beforeTaskId)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| beforeTaskId | Int32 | 将在其之前插入当前任务的任务的 Id（[`Id`](../../tsk/id/)）。 |

## 示例

展示如何使用任务的 Id 在相同的父级下移动任务。

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// 将 ID 为 5 的任务移动到 ID 为 3 的任务之前
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// 或
// 将任务移动到集合的末尾
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


