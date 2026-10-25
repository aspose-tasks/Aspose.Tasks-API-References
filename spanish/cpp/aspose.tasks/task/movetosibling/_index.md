---
title: "Aspose::Tasks::Task::MoveToSibling método"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks for C++"
description: "Mueve la tarea actual al mismo Nivel de Esquema antes de la tarea especificada."
type: docs
weight: 1370
url: /es/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Mueve la tarea actual al mismo nivel de esquema antes de la tarea especificada. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, trabajo y campos de costo, niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo, recalcula ids y niveles de esquema).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parámetro | Descripción |
| --- | --- |
| beforeTask | Tarea antes de la cual se insertará la tarea actual. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Mueve la tarea actual al mismo Nivel de Esquema antes de una tarea con el Id especificado. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, campos de trabajo y costo, niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma todas las tareas del proyecto automáticamente (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, campos de trabajo y costo, recalcula ids y niveles de esquema).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parámetro | Descripción |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) de una tarea antes de la cual se insertará la tarea actual. |

