---
title: "Task.ExternalUid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает или задает уникальный идентификатор внешних задач, когда задача является внешней"
type: docs
weight: 430
url: /ru/net/aspose.tasks/task/externaluid/
---
## Task.ExternalUid property

Получает или задает уникальный идентификатор внешней задачи, когда задача является внешней.

```csharp
public int ExternalUid { get; set; }
```

## Примеры

Показывает, как создать связь задачи между проектами — ссылку на задачу в другом (внешнем) проекте.

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Чтобы создать ссылку на задачу из другого проекта, необходимо создать
// ее дубликат (или «внешнюю») задачу в текущем проекте.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


