---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete 方法"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks for C++"
description: "将整个项目的所有工作更新为截至指定日期的已完成状态。"
type: docs
weight: 2080
url: /zh/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

将整个项目的所有工作更新为截至指定日期的已完成状态。

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| completeThrough | 用于将工作更新为已完成的日期。 |
| setZeroOrHundredPercentCompleteOnly | 如果设置为 true，则仅将完成日期早于指定的 complete-through 日期的任务更新为 100% 完成。否则，根据计划的开始日期和 complete-through 日期计算完成百分比值。 |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

将指定任务列表的所有工作更新为在指定日期之前完成。

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| completeThrough | 用于将工作更新为已完成的日期。 |
| setZeroOrHundredPercentCompleteOnly | 如果设置为 true，则仅将完成日期早于指定的 complete-through 日期的任务更新为 100% 完成。否则，根据计划的开始日期和 complete-through 日期计算完成百分比值。 |
| taskCollection | 用于更新工作任务的 List< Task > 列表。 |

