---
title: "TaskStatus"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Especifica el estado de una tarea."
type: docs
weight: 301
url: /es/java/com.aspose.tasks/taskstatus/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TaskStatus extends System.Enum
```

Especifica el estado de una tarea.
## Campos

| Campo | Descripción |
| --- | --- |
| [Complete](#Complete) | La tarea está 100 por ciento completa. |
| [Future](#Future) | El estado de tarea 'Future' se establece cuando la fecha de inicio de la tarea es mayor que la fecha de estado. |
| [Late](#Late) | La tarea está atrasada si el porcentaje acumulado por fases de tiempo no alcanza la medianoche del día anterior a la fecha de estado. |
| [OnSchedule](#OnSchedule) | La tarea está dentro del cronograma si el porcentaje acumulado por fases de tiempo se extiende al menos hasta el día anterior a la fecha de estado. |
| [Undefined](#Undefined) | Estado de tarea indefinido. |
### Complete {#Complete}
```
public static final int Complete
```


La tarea está 100 por ciento completa.

### Future {#Future}
```
public static final int Future
```


El estado de tarea 'Future' se establece cuando la fecha de inicio de la tarea es mayor que la fecha de estado.

### Late {#Late}
```
public static final int Late
```


La tarea está atrasada si el porcentaje acumulado por fases de tiempo no alcanza la medianoche del día anterior a la fecha de estado.

### OnSchedule {#OnSchedule}
```
public static final int OnSchedule
```


La tarea está dentro del cronograma si el porcentaje acumulado por fases de tiempo se extiende al menos hasta el día anterior a la fecha de estado.

### Undefined {#Undefined}
```
public static final int Undefined
```


Estado de tarea indefinido.

