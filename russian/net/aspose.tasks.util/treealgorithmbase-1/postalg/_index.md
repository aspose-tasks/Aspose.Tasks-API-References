---
title: "TreeAlgorithmBase1.PostAlg"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TreeAlgorithmBase. Вызывается после обработки узла дерева."
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/treealgorithmbase-1/postalg/
---
## TreeAlgorithmBase&lt;T&gt;.PostAlg method

Вызывается после обработки узла дерева.

```csharp
public virtual void PostAlg(T el, int level)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | T | Узел для обработки. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


