---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete método"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks for C++"
description: "Actualiza todo el trabajo como completado hasta una fecha especificada para todo el proyecto."
type: docs
weight: 2080
url: /es/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Actualiza todo el trabajo como completado hasta una fecha especificada para todo el proyecto.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parámetro | Descripción |
| --- | --- |
| completeThrough | La fecha para actualizar el trabajo como completado hasta. |
| setZeroOrHundredPercentCompleteOnly | Si se establece en true, actualiza solo aquellas tareas como 100 % completadas cuya fecha de finalización sea anterior a la fecha de completado especificada. De lo contrario, calcula un valor de porcentaje completado basado en las fechas de inicio programadas y de completado. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Actualiza todo el trabajo como completado hasta una fecha especificada para la lista de tareas especificada.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parámetro | Descripción |
| --- | --- |
| completeThrough | La fecha para actualizar el trabajo como completado hasta. |
| setZeroOrHundredPercentCompleteOnly | Si se establece en true, actualiza solo aquellas tareas como 100 % completadas cuya fecha de finalización sea anterior a la fecha de completado especificada. De lo contrario, calcula un valor de porcentaje completado basado en las fechas de inicio programadas y de completado. |
| taskCollection | Lista< Task > de tareas para las que actualizar el trabajo. |

