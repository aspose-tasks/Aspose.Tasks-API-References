---
title: "Класс RiskPatternCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.RiskAnalysis.RiskPatternCollection. Представляет коллекцию, содержащую экземпляры класса RiskPattern."
type: docs
weight: 1940
url: /ru/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

Представляет коллекцию, содержащую экземпляры класса [`RiskPattern`](../riskpattern/).

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | Получает экземпляр класса [`RiskPattern`](../riskpattern/) для указанной задачи. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | Добавляет экземпляр класса [`RiskPattern`](../riskpattern/) в эту коллекцию. |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | Удаляет первое вхождение конкретного объекта из этой коллекции. |

## Примеры

Показывает, как работать с коллекциями шаблонов риска.

```csharp
var settings = new RiskAnalysisSettings
{
    // Установите количество итераций для моделирования Монте-Карло (значение по умолчанию — 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// поскольку RiskPatternCollection не является только для чтения
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// можно добавить новые шаблоны 
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// перебрать добавленные шаблоны
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// отредактировать шаблон в коллекции, используя доступ по индексу
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// проверьте шаблоны после редактирования
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// мы можем удалить шаблон
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// проверьте, что шаблон отсутствует в коллекции
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// коллекцию можно очистить двумя способами

// скопировать шаблоны в массив и удалять их по одному
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// или можно полностью очистить коллекцию шаблонов
settings.Patterns.Clear();
```

### См. также

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


