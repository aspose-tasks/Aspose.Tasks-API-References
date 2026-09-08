---
title: "Перечисление ConfidenceLevel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.RiskAnalysis.ConfidenceLevel. Указывает поддерживаемые уровни доверия, используемые в анализе рисков, которые соответствуют проценту времени, когда фактические значения находятся в пределах оптимистических и пессимистических оценок."
type: docs
weight: 1850
url: /ru/net/aspose.tasks.riskanalysis/confidencelevel/
---
## ConfidenceLevel enumeration

Указывает поддерживаемые уровни доверия, используемые в анализе рисков, которые соответствуют проценту времени, когда фактические значения находятся в пределах оптимистических и пессимистических оценок.

```csharp
public enum ConfidenceLevel
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| CL99 | `99` | Уровень доверия 99 %. |
| CL95 | `95` | Уровень доверия 95 %. |
| CL90 | `90` | Уровень доверия 90 %. |
| CL85 | `85` | Уровень доверия 85 %. |
| CL75 | `75` | Уровень доверия 75 %. |

## Примеры

Показывает, как начать анализ рисков, используя &lt;see cref=\"Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings\" /&gt;.

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// изменить настройки
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

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


