---
title: "Класс RiskPattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.RiskAnalysis.RiskPattern. Представляет шаблон риска для задачи проекта."
type: docs
weight: 1930
url: /ru/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Представляет шаблон риска для задачи проекта.

```csharp
public class RiskPattern
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | Инициализирует новый экземпляр класса `RiskPattern`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Получает или задает уровень доверия, соответствующий проценту времени, когда фактические сгенерированные значения будут находиться в пределах оптимистических и пессимистических оценок. Значение по умолчанию — CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Получает или задает распределение вероятностей, используемое в моделировании Монте‑Карло. Значение по умолчанию — ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | Получает или задает процент наиболее вероятной продолжительности задачи, который может реализоваться в наилучшем сценарии проекта. Значение по умолчанию — 75, что означает, что если оценочная продолжительность задачи составляет 4 дня, то оптимистичная продолжительность будет 3 дня. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | Получает или задает процент наиболее вероятной продолжительности задачи, который может реализоваться в наихудшем сценарии проекта. Значение по умолчанию — 125, что означает, что если оценочная продолжительность задачи составляет 4 дня, то пессимистичная продолжительность будет 5 дней. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Получает задачу проекта, к которой применяется данный шаблон риска. |

## Примеры

Показывает, как определить настройки симуляции риска.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

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

settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### См. также

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


