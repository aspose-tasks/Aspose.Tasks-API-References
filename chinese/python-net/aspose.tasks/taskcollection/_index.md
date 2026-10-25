---
title: "TaskCollection"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 1140
url: /zh/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

表示一个 [Task](/tasks/python-net/aspose.tasks/task/) 对象的集合。

TaskCollection 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| parent_project | 获取 TaskCollection 对象的父项目。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| add() | 将指定任务添加到 [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) 类的实例中。<br/>            如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如时差、工作和成本字段、ID 和大纲级别等依赖字段）。<br/>            如果 ParentProject.CalculationMode 为 Manual，方法将仅自动计算任务 ID、大纲级别和大纲编号。<br/>            如果 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务<br/>            （开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段，重新计算 ID 和大纲级别）。 |
| add(task_name) | 向子任务集合中添加一个新任务。 |
| add(task_name, before_task_id) |  |
| add(parameters) | 在具有指定 ID 且位于相同大纲级别的任务之前插入一个新任务。 |
| to_list() | 将 TaskCollection 对象转换为 [Task](/tasks/python-net/aspose.tasks/task/) 对象的列表。 |
| get_by_uid(uid) | 返回具有指定 Uid 的任务，该任务的祖先是此集合的父任务。 |
| get_by_id(id) | 返回具有指定 Id 的任务，该任务的祖先是此集合的父任务。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

