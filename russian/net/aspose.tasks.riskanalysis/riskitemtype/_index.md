---
title: "Перечисление RiskItemType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.RiskAnalysis.RiskItemType перечисление. Указывает поля задачи, для которых собирается статистическая информация во время анализа рисков."
type: docs
weight: 1920
url: /ru/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

Указывает поля задач, для которых собирается статистическая информация во время анализа рисков.

```csharp
public enum RiskItemType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Start | `0` | Начало задачи. |
| Finish | `1` | Завершение задачи. |
| EarlyStart | `2` | Раннее начало задачи. |
| EarlyFinish | `3` | Раннее завершение задачи. |
| LateStart | `4` | Позднее начало задачи. |
| LateFinish | `5` | Позднее завершение задачи. |

## Примеры

Показывает, как вычислить статистику рисков и сохранить её в виде PDF‑отчёта.

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

// сохранить анализ как отчёт в файл по пути к файлу
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// или сохранить анализ в поток
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### См. также

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


