---
title: "TaskLink.LinkType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLink. Возвращает или задает тип ссылки"
type: docs
weight: 60
url: /ru/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Получает или задает тип ссылки.

```csharp
public TaskLinkType LinkType { get; set; }
```

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

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


