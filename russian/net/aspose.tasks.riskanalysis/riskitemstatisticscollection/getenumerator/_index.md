---
title: "RiskItemStatisticsCollection.GetEnumerator"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод RiskItemStatisticsCollection. Возвращает перечислитель для этой коллекции."
type: docs
weight: 20
url: /ru/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/getenumerator/
---
## RiskItemStatisticsCollection.GetEnumerator method

Возвращает перечислитель для этой коллекции.

```csharp
public IEnumerator<RiskItemStatistics> GetEnumerator()
```

### Возвращаемое значение

перечислитель для этой коллекции.

## Примеры

Показывает, как работать с коллекцией статистики рисков.

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

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// перебрать все элементы статистики
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// или получить конкретную статистику
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### См. также

* class [RiskItemStatistics](../../riskitemstatistics/)
* class [RiskItemStatisticsCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatisticscollection/)
* assembly [Aspose.Tasks](../../../)


