---
title: "RiskPattern"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un patrón de riesgo para una tarea del proyecto."
type: docs
weight: 268
url: /es/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Representa un patrón de riesgo para una tarea del proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Inicializa una nueva instancia de la clase [RiskPattern](../../com.aspose.tasks/riskpattern). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Obtiene el nivel de confianza que corresponde al porcentaje del tiempo en que los valores generados realmente estarán dentro de las estimaciones optimistas y pesimistas. |
| [getDistribution()](#getDistribution--) | Obtiene la distribución de probabilidad utilizada en la simulación Monte Carlo. |
| [getOptimistic()](#getOptimistic--) | Obtiene el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto. |
| [getPessimistic()](#getPessimistic--) | Obtiene el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto. |
| [getTask()](#getTask--) | Obtiene una tarea del proyecto a la que se aplica este patrón de riesgo. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Establece el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados realmente estarán dentro de las estimaciones optimistas y pesimistas. |
| [setDistribution(int value)](#setDistribution-int-) | Establece la distribución de probabilidad utilizada en la simulación Monte Carlo. |
| [setOptimistic(int value)](#setOptimistic-int-) | Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto. |
| [setPessimistic(int value)](#setPessimistic-int-) | Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Inicializa una nueva instancia de la clase [RiskPattern](../../com.aspose.tasks/riskpattern).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | la tarea del proyecto especificada para la cual se aplicará este riesgo en la simulación Monte Carlo. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Obtiene el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados realmente estarán dentro de las estimaciones optimistas y pesimistas. El valor predeterminado es CL99.

--------------------

Puede ser uno de los valores definidos en el `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) enumeración.

**Returns:**
int - el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados realmente estarán dentro de las estimaciones optimistas y pesimistas.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Obtiene la distribución de probabilidad utilizada en la simulación Monte Carlo. El valor predeterminado es ProbabilityDistributionType.Normal.

--------------------

Puede ser uno de los valores definidos en la [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enumeración.

**Returns:**
int - la distribución de probabilidad utilizada en la simulación Monte Carlo.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Obtiene el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto. El valor predeterminado es 75, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración optimista será de 3 días.

**Returns:**
int - el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Obtiene el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto. El valor predeterminado es 125, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración pesimista será de 5 días.

**Returns:**
int - el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto.
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtiene una tarea del proyecto a la que se aplica este patrón de riesgo.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Establece el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados realmente estarán dentro de las estimaciones optimistas y pesimistas. El valor predeterminado es CL99.

--------------------

Puede ser uno de los valores definidos en el `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) enumeración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el nivel de confianza que corresponde al porcentaje de tiempo en que los valores generados realmente estarán dentro de las estimaciones optimistas y pesimistas. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Establece la distribución de probabilidad utilizada en la simulación Monte Carlo. El valor predeterminado es ProbabilityDistributionType.Normal.

--------------------

Puede ser uno de los valores definidos en la [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enumeración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la distribución de probabilidad utilizada en la simulación Monte Carlo. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto. El valor predeterminado es 75, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración optimista será de 3 días.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el porcentaje de la duración de tarea más probable que puede ocurrir en el mejor escenario posible del proyecto. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Establece el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto. El valor predeterminado es 125, lo que significa que si la duración estimada de la tarea especificada es de 4 días, entonces la duración pesimista será de 5 días.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el porcentaje de la duración de tarea más probable que puede ocurrir en el peor escenario posible del proyecto. |

