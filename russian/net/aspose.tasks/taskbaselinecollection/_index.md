---
title: "Класс TaskBaselineCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskBaselineCollection. Представляет коллекцию объектов TaskBaseline"
type: docs
weight: 2380
url: /ru/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Представляет коллекцию объектов [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте TaskBaselineCollection. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Удаляет базовую линию из этой коллекции. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Преобразует объект TaskBaselineCollection в список объектов [`TaskBaseline`](../taskbaseline/). |

## Примеры

Показывает, как работать с коллекциями базовых линий задач.

```csharp
var project = new Project();

// создать базовые линии проекта
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// печать базовых линий задач
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// давайте очистим все базовые линии
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### См. также

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


