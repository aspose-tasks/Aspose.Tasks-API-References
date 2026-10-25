---
title: "RiskPattern"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 60
url: /es/python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

Representa un patrón de riesgo para una tarea de proyecto.

El tipo RiskPattern expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| RiskPattern(task) | Inicializa una nueva instancia de la clase [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/). |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| task | Obtiene una tarea del proyecto a la que se aplica este patrón de riesgo. |
| distribución | Obtiene o establece la distribución de probabilidad utilizada en la simulación Monte Carlo.<br/>            El valor predeterminado es ProbabilityDistributionType.Normal. |
| confidence_level | Obtiene o establece el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados reales estarán dentro de las estimaciones optimista y pesimista.<br/>            El valor predeterminado es CL99. |
| optimistic | Obtiene o establece el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto.<br/>            El valor predeterminado es 75, lo que significa que si la duración estimada especificada de la tarea es de 4 días, entonces la duración optimista será de 3 días. |
| pessimistic | Obtiene o establece el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto.<br/>            El valor predeterminado es 125, lo que significa que si la duración estimada especificada de la tarea es de 4 días, entonces la duración pesimista será de 5 días. |

### Ver también

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)

