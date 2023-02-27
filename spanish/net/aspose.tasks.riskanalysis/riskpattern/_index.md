---
title: Class RiskPattern
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.RiskAnalysis.RiskPattern clase. Representa un patrón de riesgo para una tarea de proyecto.
type: docs
weight: 1670
url: /es/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Representa un patrón de riesgo para una tarea de proyecto.

```csharp
public class RiskPattern
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | Inicializa una nueva instancia del`RiskPattern` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Obtiene o establece el nivel de confianza que corresponde al porcentaje de tiempo en que los valores reales generados estarán dentro de las estimaciones optimistas y pesimistas. El valor predeterminado es CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Obtiene o establece la distribución de probabilidad utilizada en la simulación Monte Carlo. El valor predeterminado es ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | Obtiene o establece el porcentaje de la duración más probable de la tarea que puede ocurrir en el mejor escenario posible del proyecto. El valor predeterminado es 75, lo que significa que si la duración estimada de la tarea especificada es de 4 días, la duración optimista será de 3 días. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | Obtiene o establece el porcentaje de la duración más probable de la tarea que puede ocurrir en el peor escenario posible del proyecto. El valor predeterminado es 125, lo que significa que si la duración estimada de la tarea especificada es de 4 días, la duración pesimista será de 5 días. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Obtiene una tarea de proyecto a la que se aplica este patrón de riesgo. |

### Ver también

* espacio de nombres [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* asamblea [Aspose.Tasks](../../)


