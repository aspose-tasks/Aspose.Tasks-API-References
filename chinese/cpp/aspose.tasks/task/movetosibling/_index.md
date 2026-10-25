---
title: "Aspose::Tasks::Task::MoveToSibling 方法"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks for C++"
description: "将当前任务在相同的大纲级别上移动到指定任务之前。"
type: docs
weight: 1370
url: /zh/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

将当前任务在相同的大纲级别上移动到指定任务之前。若 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置早/晚日期）并计算诸如时差、工作和成本字段、以及大纲级别等依赖字段）。若 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 ID、大纲级别和大纲编号。若 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排整个项目的任务（开始/结束日期，设置早/晚日期，计算时差、工作和成本字段，重新计算 ID 和大纲级别）。

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| beforeTask | 将在其之前插入当前任务的任务。 |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

将当前任务在相同的大纲级别上移动到具有指定 Id 的任务之前。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置早/晚日期）并计算诸如剩余时间、工作和成本字段、以及大纲级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，则该方法仅自动计算任务 id、大纲级别和大纲编号。如果 ParentProject.CalculationMode 为 Automatic，则该方法会自动重新安排所有项目任务（开始/结束日期，设置早/晚日期，计算剩余时间、工作和成本字段，重新计算 id 和大纲级别）。

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| beforeTaskId | 在其之前插入当前任务的任务的 Id ( Tsk::Id )。 |

