---
title: Task.MoveToSibling
second_title: Aspose.Tasks for .NET API 参考
description: Task 方法. 将当前任务移动到指定任务之前的同一大纲级别 如果 ParentProject.CalculationMode 为 None用户应在使用此方法后调用 Project.Recalculate它将重新安排所有项目任务开始/完成日期设置早/迟到日期并计算相关字段如工作时间工作和成本字段大纲级别 如果 ParentProject.CalculationMode 是手动的该方法将仅自动计算任务 ID大纲级别和大纲编号 如果 ParentProject.CalculationMode 是自动的该方法自动重新安排所有项目的任务 开始/结束日期设置早/晚日期计算松弛时间工作和成本字段重新计算 ID 和大纲级别
type: docs
weight: 1370
url: /zh/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

将当前任务移动到指定任务之前的同一大纲级别。 如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/完成日期，设置早/迟到日期）并计算相关字段，如工作时间、工作和成本字段、大纲级别）。 如果 ParentProject.CalculationMode 是手动的，该方法将仅自动计算任务 ID、大纲级别和大纲编号。 如果 ParentProject.CalculationMode 是自动的该方法自动重新安排所有项目的任务 （开始/结束日期、设置早/晚日期、计算松弛时间、工作和成本字段、重新计算 ID 和大纲级别）。

```csharp
public void MoveToSibling(Task beforeTask)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| beforeTask | Task | 将插入当前任务的任务。 |

### 也可以看看

* class [Task](../)
* 命名空间 [Aspose.Tasks](../../task/)
* 部件 [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

将当前任务移动到具有指定 Id 的任务之前的相同大纲级别。 如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置早/晚日期）并计算相关字段，例如 slacks、工作和成本字段、大纲级别）。 如果 ParentProject.CalculationMode 为手动，则该方法将仅自动计算任务 ID、大纲级别和大纲编号。 如果 ParentProject. CalculationMode 是 Automatic 该方法自动重新安排所有项目的任务 （开始/结束日期、设置早/晚日期、计算 slacks、工作和成本字段、重新计算 ID 和大纲级别）。

```csharp
public void MoveToSibling(int beforeTaskId)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| beforeTaskId | Int32 | ID （[`Id`](../../tsk/id/)) 之前将插入当前任务的任务。 |

### 也可以看看

* class [Task](../)
* 命名空间 [Aspose.Tasks](../../task/)
* 部件 [Aspose.Tasks](../../../)


