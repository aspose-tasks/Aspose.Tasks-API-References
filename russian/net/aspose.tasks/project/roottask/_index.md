---
title: "Project.RootTask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Возвращает корень дерева задач"
type: docs
weight: 800
url: /ru/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Получает корень дерева задач.

```csharp
public Task RootTask { get; }
```

## Примеры

Показывает, как добавить задачу в проект, используя корневую задачу проекта.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### См. также

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


