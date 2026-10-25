---
title: "LevelingOrder"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Define los valores posibles del orden de nivelación."
type: docs
weight: 143
url: /es/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Define los valores posibles del orden de nivelación.
## Campos

| Campo | Descripción |
| --- | --- |
| [IdOnly](#IdOnly) | Las tareas se retrasan en orden ascendente de Id. |
| [PriorityThenStandard](#PriorityThenStandard) | La prioridad se considera primero, luego las mismas propiedades que en Standard. |
| [Standard](#Standard) | Se tienen en cuenta las siguientes propiedades: relaciones de predecesores, holgura total (una tarea con mayor holgura total se retrasa primero), fecha de inicio, prioridad. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Las tareas se retrasan en orden ascendente de Id.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


La prioridad se considera primero, luego las mismas propiedades que en Standard.

### Standard {#Standard}
```
public static final int Standard
```


Se tienen en cuenta las siguientes propiedades: relaciones de predecesores, holgura total (una tarea con mayor holgura total se retrasa primero), fecha de inicio, prioridad. Este es el valor predeterminado.

