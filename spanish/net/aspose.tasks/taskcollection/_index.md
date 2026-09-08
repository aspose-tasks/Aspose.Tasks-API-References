---
title: "Clase TaskCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskCollection. Representa una colección de objetos Task"
type: docs
weight: 2390
url: /es/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Representa una colección de [`Task`](../task/) objetos.

```csharp
public class TaskCollection : IList<Task>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Obtiene el número de objetos contenidos en la TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Obtiene el proyecto padre del objeto TaskCollection. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema de la última tarea. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Inserta una nueva tarea antes de una tarea con el id especificado y en el mismo nivel de esquema. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Agrega una nueva tarea a la colección de tareas hijas. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Agregue la tarea especificada a la instancia de la clase `TaskCollection`. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, campos de trabajo y costo, ids y niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, campos de trabajo y costo, recalcula ids y niveles de esquema). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Agrega una nueva tarea recurrente a la colección de tareas hijas. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Comprueba si la colección contiene el elemento especificado. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Devuelve una tarea con el Id especificado cuyo ancestro es la tarea padre de esta colección. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Devuelve una tarea con el Uid especificado cuyo ancestro es la tarea padre de esta colección. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Esta es la implementación de sustituto del método Insert de IList, que solo lanza NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Esta es la implementación de sustituto del método Remove de ICollection, que solo lanza NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Convierte el objeto TaskCollection a una lista de objetos [`Task`](../task/). |

## Ejemplos

Muestra cómo trabajar con colecciones de tareas.

```csharp
var project = new Project();

// la colección de tareas no es de solo lectura y puede ser ampliada
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// crear tareas
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// imprimir tareas del proyecto
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// una tarea puede obtenerse de la colección por ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// o por UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// también se puede agregar una tarea recurrente
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// se devuelve la primera tarea de una secuencia
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// la colección puede convertirse en una lista simple
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Ver también

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


