---
title: "RiskPatternCollection.IsReadOnly"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RiskPatternCollection. Возвращает значение, указывающее, является ли эта коллекция только для чтения; иначе false."
type: docs
weight: 20
url: /ru/net/aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/
---
## RiskPatternCollection.IsReadOnly property

Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false.

```csharp
public bool IsReadOnly { get; }
```

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

* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


