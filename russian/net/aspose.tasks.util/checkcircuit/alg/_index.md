---
title: "CheckCircuit.Alg"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CheckCircuit. Проверяет, был ли указанный объект уже обработан"
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Проверьте, был ли указанный объект уже обработан.

```csharp
public override void Alg(Task el, int level)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | Задача | Объект для обработки. |
| уровень | Int32 | Уровень узла дерева. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


