---
title: WorkingTime.WorkingTime
second_title: Referencia de Aspose.Tasks para la API de .NET
description: WorkingTime constructor. Inicializa una nueva instancia delWorkingTime clase con un intervalo con las horas de inicio y finalización especificadas.
type: docs
weight: 10
url: /es/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Inicializa una nueva instancia del[`WorkingTime`](../) clase con un intervalo con las horas de inicio y finalización especificadas.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fromTime | DateTime | hora de inicio del intervalo |
| toTime | DateTime | hora de finalización del intervalo |

### Ver también

* class [WorkingTime](../)
* espacio de nombres [Aspose.Tasks](../../workingtime/)
* asamblea [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Inicializa una nueva instancia del[`WorkingTime`](../) clase con un elemento de intervalo con las horas de inicio y finalización especificadas.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fromTime | TimeSpan | Hora de inicio del intervalo representada porTimeSpan estructura |
| toTime | TimeSpan | Hora de finalización del intervalo representada porTimeSpan estructura |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Cuando toTime es menor que o igual a toTime argument o cuando el intervalo entre fromTime y toTime es mayor a 24 horas. |

### Ejemplos

La sobrecarga de WorkingTime ctor se puede usar para inicializar el inicio y el final del intervalo usando TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Ver también

* class [WorkingTime](../)
* espacio de nombres [Aspose.Tasks](../../workingtime/)
* asamblea [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Inicializa una nueva instancia del[`WorkingTime`](../) clase con un elemento de intervalo con las horas de inicio y finalización especificadas.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fromHours | Int32 | Hora de inicio del intervalo representada por un número entero de horas (0-24). |
| toHours | Int32 | Hora de finalización del intervalo representada por un número entero de horas (0-24). |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Cuando toTime es menor que o igual a toTime argument o cuando el intervalo entre fromTime y toTime es mayor a 24 horas. |

### Ejemplos

La sobrecarga de WorkingTime ctor se puede usar para inicializar el inicio y el final del intervalo usando horas enteras:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### Ver también

* class [WorkingTime](../)
* espacio de nombres [Aspose.Tasks](../../workingtime/)
* asamblea [Aspose.Tasks](../../../)


