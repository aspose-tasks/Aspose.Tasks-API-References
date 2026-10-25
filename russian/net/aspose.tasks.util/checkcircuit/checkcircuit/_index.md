---
title: "CheckCircuit.CheckCircuit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор CheckCircuit. Инициализирует новый экземпляр класса CheckCircuit"
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Инициализирует новый экземпляр класса [`CheckCircuit`](../).

```csharp
public CheckCircuit()
```

## Примеры

Показывает, как обнаружить повреждённую структуру проекта.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// проверьте структуру проекта.
// Будет выброшено <see cref=\"TasksException\">, если структура проекта некорректна.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### См. также

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


