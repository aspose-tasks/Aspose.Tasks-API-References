---
title: "Aspose::Tasks::Project::Recalculate método"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks for C++"
description: "Reprograma todos los IDs de tareas del proyecto, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo."
type: docs
weight: 1130
url: /es/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Reprograma todos los IDs de tareas del proyecto, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Reprograma todos los IDs de tareas del proyecto, niveles de esquema, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, campos de trabajo y costo con validación opcional.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Parámetro | Descripción |
| --- | --- |
| validar | Si es verdadero, se realizará la validación de recalculación. Qué datos se validan: En este momento solo se implementa la validación básica de los rangos de fechas de tareas y enlaces de tareas. Los rangos de fechas de la tarea (p. ej., ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) así como las fechas de los enlaces de tareas se comprobarán contra el criterio de que la fecha de inicio sea menor o igual que la fecha de fin. Si alguna de las condiciones descritas arriba falla, se lanzará la excepción RecalculationValidationException. |

