---
title: "Tsk.ExternalId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Если задача является внешней, оно содержит внешний идентификатор задачи"
type: docs
weight: 360
url: /ru/net/aspose.tasks/tsk/externalid/
---
## Tsk.ExternalId field

Если задача является внешней, она содержит внешний идентификатор задачи.

```csharp
public static readonly Key<int, TaskKey> ExternalId;
```

## Примеры

Показывает, как идентифицировать задачи, связанные между проектами.

```csharp
var project = new Project(DataDir + "External.mpp");
var externalTask = project.RootTask.Children.GetByUid(1);

// Показать идентификатор задачи во внешнем проекте
Console.WriteLine(externalTask.Get(Tsk.Id).ToString());

// Показать идентификатор задачи в оригинальном проекте
Console.WriteLine(externalTask.Get(Tsk.ExternalId).ToString());
```

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


