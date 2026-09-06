---
title: "WorkingTime"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un horario de trabajo durante un día de la semana."
type: docs
weight: 365
url: /es/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Representa un horario de trabajo durante un día de la semana.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Inicializa una nueva instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime) con un intervalo con los tiempos de inicio y fin especificados. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Inicializa una nueva instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime) con un elemento de intervalo con los tiempos de inicio y fin especificados. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Inicializa una nueva instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime) con un elemento de intervalo con los tiempos de inicio y fin especificados. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Comprueba que los objetos sean iguales. |
| [getFrom()](#getFrom--) | Obtiene el comienzo de un tiempo de trabajo. |
| [getTo()](#getTo--) | Obtiene el final de un tiempo de trabajo. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Inicializa una nueva instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime) con un intervalo con los tiempos de inicio y fin especificados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fromTime | java.util.Date | tiempo de inicio del intervalo |
| toTime | java.util.Date | tiempo de fin del intervalo |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Inicializa una nueva instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime) con un elemento de intervalo con los tiempos de inicio y fin especificados.

--------------------

&gt; ```
&gt; La sobrecarga del ctor WorkingTime puede usarse para inicializar el inicio y fin del intervalo usando TimeSpans:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fromHours | int | Tiempo de inicio del intervalo representado por un número entero de horas (0-24). |
| toHours | int | Tiempo de fin del intervalo representado por un número entero de horas (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Comprueba que los objetos sean iguales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | Segundo objeto a comparar. |

**Returns:**
boolean - Verdadero si los objetos son iguales, falso de lo contrario.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Obtiene el comienzo de un tiempo de trabajo.

**Returns:**
java.util.Date - el comienzo de un tiempo de trabajo.
### getTo() {#getTo--}
```
public final Date getTo()
```


Obtiene el final de un tiempo de trabajo.

**Returns:**
java.util.Date - el final de un tiempo de trabajo.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
int - devuelve un valor de código hash para este objeto.
