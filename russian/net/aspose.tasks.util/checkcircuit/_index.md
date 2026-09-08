---
title: "Класс CheckCircuit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Util.CheckCircuit. Проверяет дерево задач на наличие цикла"
type: docs
weight: 2680
url: /ru/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Проверяет дерево (задач) на наличие цикла.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Инициализирует новый экземпляр класса `CheckCircuit`. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Проверьте, был ли указанный объект уже обработан. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


