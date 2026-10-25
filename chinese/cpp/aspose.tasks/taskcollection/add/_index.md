---
title: "Aspose::Tasks::TaskCollection::Add 方法"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "在与上一个任务相同的大纲级别上向项目任务集合中添加新任务。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

在与上一个任务相同的大纲级别上向项目任务集合中添加新任务。

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

在具有指定 ID 的任务之前并在相同的大纲级别插入新任务。

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 参数 | 用于创建循环任务的指定参数。 |

---

## Add (3 of 5) {#add_3}

将指定的任务添加到 TaskCollection 类的实例中。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置早/晚日期）并计算诸如浮动、工作和成本字段、ID 以及大纲级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，则该方法仅自动计算任务 ID、大纲级别和大纲编号。如果 ParentProject.CalculationMode 为 Automatic，则该方法自动重新安排所有项目任务（开始/结束日期，设置早/晚日期，计算浮动、工作和成本字段，重新计算 ID 和大纲级别）。

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 项目 | 应添加到此任务集合的指定任务。 |

---

## Add (4 of 5) {#add_4}

向子任务集合添加新任务。

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| taskName | 指定的任务名称。 |

---

## Add (5 of 5) {#add_5}

向子任务集合添加新循环任务。

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| taskName | 指定的任务名称。 |
| beforeTaskId | 在其前插入新任务的指定任务 ID。 |

