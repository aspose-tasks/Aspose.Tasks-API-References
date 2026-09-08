---
title: "Класс RiskAnalysisSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings класс. Указывает настройки для выполнения анализа рисков."
type: docs
weight: 1880
url: /ru/net/aspose.tasks.riskanalysis/riskanalysissettings/
---
## RiskAnalysisSettings class

Указывает настройки для выполнения анализа рисков.

```csharp
public class RiskAnalysisSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RiskAnalysisSettings](riskanalysissettings/)() | Инициализирует новый экземпляр класса `RiskAnalysisSettings`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IterationsCount](../../aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/) { get; set; } | Получает или задает количество итераций, используемых в моделировании Монте-Карло. Значение по умолчанию — 100. |
| [Patterns](../../aspose.tasks.riskanalysis/riskanalysissettings/patterns/) { get; } | Получает коллекцию, содержащую экземпляры класса [`RiskPattern`](../riskpattern/). |

## Примеры

Показывает, как подготовить настройки анализа рисков для симуляций Монте-Карло.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Установите количество итераций для моделирования Монте-Карло (значение по умолчанию — 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Инициализировать шаблон риска
var pattern = new RiskPattern(task);

// Выберите тип распределения для генератора случайных чисел, из которого будут генерироваться возможные значения (в настоящее время поддерживаются только два типа: нормальное и равномерное)            
// Для получения дополнительных сведений см. здесь: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Установите процент наиболее вероятной продолжительности задачи, который может произойти в наилучшем сценарии проекта 
// Значение по умолчанию равно 75, что означает, что если оценочная продолжительность задачи составляет 4 дня, то оптимистичная продолжительность будет 3 дня
pattern.Optimistic = 70;

// Установите процент наиболее вероятной продолжительности задачи, который может произойти в наихудшем сценарии проекта 
// Значение по умолчанию равно 125, что означает, что если оценочная продолжительность задачи составляет 4 дня, то пессимистичная продолжительность будет 5 дней.
pattern.Pessimistic = 130;

// Установите уровень доверия, соответствующий проценту времени, когда фактические значения будут находиться между оптимистичными и пессимистичными оценками. 
// Можно рассматривать это как значение стандартного отклонения: чем более неопределены ваши оценки, тем больше значение стандартного отклонения, используемого в генераторе случайных чисел.
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### См. также

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


