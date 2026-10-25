---
title: "RiskAnalysisSettings.Patterns"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad RiskAnalysisSettings. Obtiene una colección que contiene las instancias de la clase RiskPattern"
type: docs
weight: 30
url: /es/net/aspose.tasks.riskanalysis/riskanalysissettings/patterns/
---
## RiskAnalysisSettings.Patterns property

Obtiene una colección que contiene las instancias de la clase [`RiskPattern`](../../riskpattern/).

```csharp
public RiskPatternCollection Patterns { get; }
```

## Ejemplos

Muestra cómo preparar la configuración del análisis de riesgos para simulaciones Monte Carlo.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Establece el número de iteraciones para la simulación Monte Carlo (el valor predeterminado es 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inicializa un patrón de riesgo
var pattern = new RiskPattern(task);

// Selecciona un tipo de distribución para el generador de números aleatorios que genere valores posibles (actualmente solo se admiten dos tipos, a saber, normal y uniforme)
// Para más detalles, consulta aquí: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto
// El valor predeterminado es 75, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración optimista será de 3 días
pattern.Optimistic = 70;

// Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto
// El valor predeterminado es 125, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración pesimista será de 5 días.
pattern.Pessimistic = 130;

// Establece un nivel de confianza que corresponde al porcentaje de tiempo en que los valores reales estarán dentro de las estimaciones optimista y pesimista.
// Puedes considerarlo como un valor de desviación estándar: cuanto más inciertas sean tus estimaciones, mayor será el valor de desviación estándar utilizado en el generador de números aleatorios.
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

### Ver también

* class [RiskPatternCollection](../../riskpatterncollection/)
* class [RiskAnalysisSettings](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysissettings/)
* assembly [Aspose.Tasks](../../../)


