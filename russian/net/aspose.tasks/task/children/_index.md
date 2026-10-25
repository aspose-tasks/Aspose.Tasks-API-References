---
title: "Task.Children"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает коллекцию дочерних задач этого объекта. Объект TaskCollection, представляющий дочерние задачи"
type: docs
weight: 190
url: /ru/net/aspose.tasks/task/children/
---
## Task.Children property

Получает коллекцию дочерних задач этого объекта. Объект TaskCollection, представляющий дочерние задачи.

```csharp
public TaskCollection Children { get; }
```

## Примеры

Показывает, как использовать коллекцию задач для добавления задачи.

```csharp
var project = new Project();

// Добавить задачу, подзадачу и сохранить проект
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### См. также

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


