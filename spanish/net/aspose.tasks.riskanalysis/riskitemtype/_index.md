---
title: "Enumeración RiskItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.RiskAnalysis.RiskItemType. Especifica los campos de tarea para los que se recopila información estadística durante el análisis de riesgos."
type: docs
weight: 1920
url: /es/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

Especifica los campos de tarea para los que se recopila la información estadística durante el análisis de riesgos.

```csharp
public enum RiskItemType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Start | `0` | Inicio de la tarea. |
| Finish | `1` | Fin de la tarea. |
| EarlyStart | `2` | Inicio temprano de la tarea. |
| EarlyFinish | `3` | Fin temprano de la tarea. |
| LateStart | `4` | Inicio tardío de la tarea. |
| LateFinish | `5` | Fin tardío de la tarea. |

## Ejemplos

Muestra cómo calcular estadísticas de riesgos y guardarlas como informe PDF.

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

// guardar el análisis como informe en un archivo mediante la ruta del archivo
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// o guardar el análisis en un flujo
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Ver también

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


