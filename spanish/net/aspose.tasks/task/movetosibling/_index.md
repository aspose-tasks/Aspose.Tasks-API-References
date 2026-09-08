---
title: "Task.MoveToSibling"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Mueve la tarea actual al mismo Nivel de esquema antes de la tarea especificada. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate después de usar este método. Reprogramará las fechas de inicio/fin de todas las tareas del proyecto, establecerá fechas tempranas/tardías y calculará los campos dependientes, como holguras, trabajo y campos de costo, y los niveles de esquema. Si ParentProject.CalculationMode es Manual, el método calculará solo el nivel de esquema del id de la tarea y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto, fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo, y recalcula los ids y los niveles de esquema."
type: docs
weight: 1370
url: /es/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Mueve la tarea actual al mismo Outline Level antes de la tarea especificada. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, trabajo y campos de costo, outline levels). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el outline level y los números de outline automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo, recalcula ids y outline levels).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| beforeTask | Tarea | Task antes del cual se insertará la tarea actual. |

## Ejemplos

Muestra cómo mover la tarea bajo el mismo padre.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Mover tareas con id 5 antes de la tarea con id 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// O
// Mover la tarea al final de la colección
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Mueve la tarea actual al mismo Outline Level antes de una tarea con el Id especificado. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, trabajo y campos de costo, outline levels). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el outline level y los números de outline automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y campos de costo, recalcula ids y outline levels).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) de una tarea antes de la cual se insertará la tarea actual. |

## Ejemplos

Muestra cómo mover la tarea bajo el mismo padre usando el Id de la tarea.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Mover tareas con id 5 antes de la tarea con id 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// O
// Mover la tarea al final de la colección
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


