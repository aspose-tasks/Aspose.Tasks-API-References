---
title: TaskCollection
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 1140
url: /python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Represents a collection of [Task](/tasks/python-net/aspose.tasks/task/) objects.

The TaskCollection type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|parent_project|Gets the parent project of the TaskCollection object.|
## Methods
| Name | Description |
| :- | :- |
|add()|Add the specified task to the instance of the [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) class.<br/>            If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, ids and outline levels).<br/>            If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically.<br/>            If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically<br/>            (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates  ids and outline levels).|
|add(task_name)|Adds a new task to children tasks collection.|
|add(task_name, before_task_id)|  |
|add(parameters)|Inserts a new task before a task with the specified id and on the same outline level.|
|to_list()|Converts the TaskCollection object to a list of [Task](/tasks/python-net/aspose.tasks/task/) objects.|
|get_by_uid(uid)|Returns a task with the specified Uid whose ancestor is parent task of this collection .|
|get_by_id(id)|Returns a task with the specified Id whose ancestor is parent task of this collection .|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

