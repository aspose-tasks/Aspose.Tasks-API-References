---
title: "Перечисление TaskLinkType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.TaskLinkType перечисление. Указывает тип зависимости задач"
type: docs
weight: 2440
url: /ru/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Указывает тип зависимости задач.

```csharp
public enum TaskLinkType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| FinishToFinish | `0` | Отношение Finish-Finish |
| FinishToStart | `1` | Отношение Finish-Start |
| StartToFinish | `2` | Отношение Start-Finish |
| StartToStart | `3` | Отношение Start-Start |

## Примеры

Показывает, как получить/установить тип ссылки задачи.

```csharp
var project = new Project();

// Добавить новые задачи
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Связать задачи с типом ссылки, установленным в Start to Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


