---
title: "RiskItemStatistics.Maximum"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RiskItemStatistics. Возвращает максимальное значение, сгенерированное в ходе моделирования Монте‑Карло"
type: docs
weight: 30
url: /ru/net/aspose.tasks.riskanalysis/riskitemstatistics/maximum/
---
## RiskItemStatistics.Maximum property

Получает максимальное значение, сгенерированное во время моделирования Монте‑Карло.

```csharp
public DateTime Maximum { get; }
```

## Примеры

Показывает, как вычислять статистику рисков.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Инициализировать шаблон риска
var pattern = new RiskPattern(task)
{
    // Выберите тип распределения для генератора случайных чисел, из которого будут генерироваться возможные значения (в настоящее время поддерживаются только два типа: нормальное и равномерное)            
    // Для получения дополнительных сведений см. здесь: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Установите процент наиболее вероятной продолжительности задачи, который может произойти в наилучшем сценарии проекта 
    // Значение по умолчанию равно 75, что означает, что если оценочная продолжительность задачи составляет 4 дня, то оптимистичная продолжительность будет 3 дня
    Optimistic = 70,

    // Установите процент наиболее вероятной продолжительности задачи, который может произойти в наихудшем сценарии проекта 
    // Значение по умолчанию равно 125, что означает, что если оценочная продолжительность задачи составляет 4 дня, то пессимистичная продолжительность будет 5 дней.
    Pessimistic = 130,

    // Установите уровень доверия, соответствующий проценту времени, когда фактические значения будут находиться между оптимистичными и пессимистичными оценками. 
    // Можно рассматривать это как значение стандартного отклонения: чем более неопределены ваши оценки, тем больше значение стандартного отклонения, используемого в генераторе случайных чисел.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Анализировать риски проекта
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### См. также

* class [RiskItemStatistics](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatistics/)
* assembly [Aspose.Tasks](../../../)


