---
title: "Aspose::Tasks::Project::Recalculate 方法"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks for C++"
description: "重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段。"
type: docs
weight: 1130
url: /zh/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段。

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算余量、工作和成本字段，并可选择进行验证。

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 验证 | 如果为 true，将执行重新计算的验证。验证哪些数据：目前仅实现对任务和任务链接日期范围的基本验证。任务的日期范围（例如 ActualStart - ActualFinish、EarlyStart - EarlyFinish 等）以及任务链接的日期将根据开始日期小于或等于结束日期的标准进行检查。如果上述任何条件失败，则会抛出 RecalculationValidationException。 |

