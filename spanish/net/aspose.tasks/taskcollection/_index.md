---
title: Class TaskCollection
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.TaskCollection clase. Representa una colección deTask objetos.
type: docs
weight: 2100
url: /es/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Representa una colección de[`Task`](../task/) objetos.

```csharp
public class TaskCollection : IList<Task>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Obtiene el número de objetos contenidos en TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Obtiene el proyecto principal del objeto TaskCollection. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema de la última tarea. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Inserta una nueva tarea antes de una tarea con la identificación especificada y en el mismo nivel de esquema. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Agrega una nueva tarea a la colección de tareas secundarias. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Agrega la tarea especificada a la instancia del`TaskCollection`class. Si ParentProject.CalculationMode es Ninguno, el usuario debe invocar Project.Recalculate() después de usar este método (reprogramará todas las tareas del proyecto (fechas de inicio/finalización, establece fechas tempranas/tardías) y calculará los campos dependientes, como horas libres, trabajo y campos de costos, ID y niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará automáticamente solo el ID de tarea, el nivel de esquema y los números de esquema. Si ParentProject.CalculationMode es Automático, el método reprograma todas las tareas del proyecto automáticamente (inicio/fin fechas, establece fechas tempranas/tardías, calcula slacks, campos de trabajo y costo, recalcula ids y niveles de esquema). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Agrega una nueva tarea recurrente a la colección de tareas secundarias. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Comprueba si la colección contiene el elemento especificado. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Devuelve una tarea con el Id especificado cuyo ancestro es la tarea principal de esta colección . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Devuelve una tarea con el Uid especificado cuyo ancestro es la tarea principal de esta colección . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Esta es la implementación de código auxiliar del método Insert de IList, que solo arroja NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Esta es la implementación de código auxiliar del método Remove de ICollection, que solo lanza NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Convierte el objeto TaskCollection en una lista de[`Task`](../task/) objetos. |

### Ver también

* class [Task](../task/)
* espacio de nombres [Aspose.Tasks](../../aspose.tasks/)
* asamblea [Aspose.Tasks](../../)


