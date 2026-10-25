---
title: "Clase RiskPattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RiskAnalysis.RiskPattern. Representa un patrón de riesgo para una tarea del proyecto"
type: docs
weight: 1930
url: /es/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Representa un patrón de riesgo para una tarea del proyecto.

```csharp
public class RiskPattern
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | Inicializa una nueva instancia de la clase `RiskPattern`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Obtiene o establece el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados reales estarán dentro de las estimaciones optimistas y pesimistas. El valor predeterminado es CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Obtiene o establece la distribución de probabilidad utilizada en la simulación Monte Carlo. El valor predeterminado es ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | Obtiene o establece el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto. El valor predeterminado es 75, lo que significa que si la duración estimada especificada de la tarea es de 4 días, entonces la duración optimista será de 3 días. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | Obtiene o establece el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto. El valor predeterminado es 125, lo que significa que si la duración estimada especificada de la tarea es de 4 días, entonces la duración pesimista será de 5 días. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Obtiene una tarea del proyecto a la que se aplica este patrón de riesgo. |

## Ejemplos

Muestra cómo definir la configuración de simulación de riesgos.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

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

### Ver también

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


