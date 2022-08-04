---
title: Task
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Representa una tarea en un proyecto.
type: docs
weight: 2060
url: /es/net/aspose.tasks/task/
---
## Task class

Representa una tarea en un proyecto.

```csharp
public class Task : IEquatable<Task>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Obtiene una colección de asignaciones de recursos para este objeto. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Obtiene o establece la colección de valores de referencia de la tarea. |
| [Children](../../aspose.tasks/task/children) { get; } | Obtiene una colección de tareas secundarias de este objeto. Objeto TaskCollection que representa las tareas secundarias. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Obtiene el objeto ExtendedAttributeCollection que contiene los valores de un atributo extendido. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Obtiene o establece[`OutlineCodeCollection`](../outlinecodecollection) objeto. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Obtiene el proyecto padre de una tarea. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Obtiene la tarea principal de una tarea. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | Obtiene un[`TaskCollection`](../taskcollection) objeto que contiene todos los predecesores de este objeto Tarea. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Obtiene la instancia de[`RecurringTaskInfo`](../recurringtaskinfo) clase para la tarea que es una tarea recurrente; si la tarea no es recurrente, devuelve nulo;  La información para la instancia de[`RecurringTaskInfo`](../recurringtaskinfo) está presente en formato de archivo mpp solamente. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Obtiene una colección SplitPart que representa las partes de una tarea. |
| [Successors](../../aspose.tasks/task/successors) { get; } | Obtiene un[`TaskCollection`](../taskcollection) objeto que contiene todos los sucesores de este objeto Tarea. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Obtiene o establece un objeto TimephasedDataCollection de esta tarea. El bloque de datos de fase temporal asociado con una tarea. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Crea una copia completa de una tarea sin subtareas. |
| [Delete](../../aspose.tasks/task/delete)() | Elimina una tarea de la colección de tareas del proyecto principal y todas sus asignaciones. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Devuelve un valor que indica si esta instancia es igual a una tarea especificada. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Devuelve el valor al que se asigna la propiedad en este contenedor. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Devuelve un valor de código hash para esta tarea. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | Devoluciones[`TimephasedDataCollection`](../timephaseddatacollection) objeto con[`TimephasedData`](./timephaseddata) valores dentro de las fechas de inicio y finalización dadas. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | Devoluciones[`TimephasedDataCollection`](../timephaseddatacollection) objeto con[`TimephasedData`](./timephaseddata) valores dentro de las fechas de inicio y finalización dadas del tipo de datos de fase temporal especificado. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Mueve la tarea actual al mismo Nivel de esquema antes de una tarea con el Id. especificado. Si ParentProject.CalculationMode es Ninguno, el usuario debe invocar Project.Recalculate() después de usar este método (reprogramará todas las tareas del proyecto (fechas de inicio/finalización, establece fechas tempranas/tardías) y calcula los campos dependientes, como espacios libres, campos de trabajo y costo, niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo la identificación de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject. CalculationMode es Automático, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/finalización, establece fechas tempranas/tardías, calcula espacios libres, campos de trabajo y costos, recalcula ID y niveles de esquema). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Mueve la tarea actual al mismo nivel de esquema antes de la tarea especificada. Si ParentProject.CalculationMode es Ninguno, el usuario debe invocar Project.Recalculate() después de usar este método (reprogramará todas las tareas del proyecto (fechas de inicio/finalización, fechas tardías) y calcule los campos dependientes, como espacios libres, campos de trabajo y costo, niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo la identificación de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automático el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/finalización, establece fechas tempranas/tardías, calcula espacios libres, campos de trabajo y costos, recalcula ids y niveles de esquema). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Sangra una tarea en el esquema. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Promueve una tarea en el esquema. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Recopila recursivamente todas las tareas secundarias de esta tarea. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Asigna la propiedad especificada al valor especificado en este contenedor. |
| override [ToString](../../aspose.tasks/task/tostring)() | Devuelve una representación de cadena corta de una tarea. Los detalles exactos de la representación no se especifican y están sujetos a cambios. |

### Observaciones

los **Tarea** está representando un plato atómico de trabajo.

Uno puede usar **Tarea**para planificar un proyecto mediante la creación de tareas y asignarles los recursos adecuados. Las tareas de un proyecto se organizan como una estructura de árbol jerárquico arraigado, con una tarea raíz y subárboles de tareas secundarias.

Para construir un árbol de tareas se puede usar una colección especializada[`TaskCollection`](../taskcollection) al acceder[`RootTask`](../project/roottask) propiedad por ejemplo:

```csharp
Project project = new Project();

// agregar nuevas tareas
Task task1 = project.RootTask.Children.Add(); // se agrega una tarea principal con un nombre vacío
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // inserta una tarea antes de childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// guarda el proyecto en uno de los formatos disponibles
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks)
* asamblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
