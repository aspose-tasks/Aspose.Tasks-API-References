---
title: "TaskLink.CrossProjectName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLink. Возвращает или задает внешний проект‑предшественник"
type: docs
weight: 10
url: /ru/net/aspose.tasks/tasklink/crossprojectname/
---
## TaskLink.CrossProjectName property

Получает или задает внешний предшествующий проект.

```csharp
public string CrossProjectName { get; set; }
```

## Примеры

Показывает, как находить ссылки задач между проектами.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// Проверить ссылки задач между проектами
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


