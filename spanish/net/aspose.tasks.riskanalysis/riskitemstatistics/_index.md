---
title: "Clase RiskItemStatistics"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RiskAnalysis.RiskItemStatistics. Representa un elemento que almacena datos estadísticos para la tarea del proyecto analizado"
type: docs
weight: 1900
url: /es/net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

Representa un elemento que almacena datos estadísticos para la tarea del proyecto analizado.

```csharp
public class RiskItemStatistics
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | Obtiene el valor esperado del elemento de riesgo. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | Obtiene una instancia de la enumeración [`RiskItemType`](../riskitemtype/). |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | Obtiene el valor máximo que se generó durante la simulación Monte Carlo. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | Obtiene el valor mínimo que se generó durante la simulación Monte Carlo. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | Obtiene la desviación estándar del elemento de riesgo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | Obtiene un valor por debajo del cual cae un porcentaje especificado de las muestras generadas. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | Devuelve una representación corta en cadena de un elemento de riesgo. Los detalles exactos de la representación no están especificados y pueden cambiar. |

## Ejemplos

Muestra cómo calcular estadísticas de riesgos.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inicializa un patrón de riesgo
var pattern = new RiskPattern(task)
{
    // Selecciona un tipo de distribución para el generador de números aleatorios que genere valores posibles (actualmente solo se admiten dos tipos, a saber, normal y uniforme)
    // Para más detalles, consulta aquí: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto
    // El valor predeterminado es 75, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración optimista será de 3 días
    Optimistic = 70,

    // Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto
    // El valor predeterminado es 125, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración pesimista será de 5 días.
    Pessimistic = 130,

    // Establece un nivel de confianza que corresponde al porcentaje de tiempo en que los valores reales estarán dentro de las estimaciones optimista y pesimista.
    // Puedes considerarlo como un valor de desviación estándar: cuanto más inciertas sean tus estimaciones, mayor será el valor de desviación estándar utilizado en el generador de números aleatorios.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Analizar los riesgos del proyecto
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

### Ver también

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


