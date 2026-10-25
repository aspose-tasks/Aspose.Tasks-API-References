---
title: "TaskCollection.Add"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskCollection. Añade la tarea especificada a la instancia de la clase TaskCollection. Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate después de usar este método. Reprogramará todas las fechas de inicio/fin de las tareas del proyecto, establecerá las fechas tempranas/tardías y calculará los campos dependientes como holguras, trabajo y costos, ids y niveles de esquema. Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y costos, recalcula ids y niveles de esquema)."
type: docs
weight: 50
url: /es/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Agrega la tarea especificada a la instancia de la clase [`TaskCollection`](../). Si ParentProject.CalculationMode es None, el usuario debe invocar Project.Recalculate() después de usar este método (Reprogramará todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías) y calculará los campos dependientes como holguras, trabajo y costos, ids y niveles de esquema). Si ParentProject.CalculationMode es Manual, el método calculará solo el id de la tarea, el nivel de esquema y los números de esquema automáticamente. Si ParentProject.CalculationMode es Automatic, el método reprograma automáticamente todas las tareas del proyecto (fechas de inicio/fin, establece fechas tempranas/tardías, calcula holguras, trabajo y costos, recalcula ids y niveles de esquema).

```csharp
public void Add(Task item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | Tarea | la tarea especificada que debe añadirse a esta colección de tareas. |

## Ejemplos

Muestra cómo mover una tarea bajo otro padre.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Obtener tareas por IDs
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Añadiendo la tarea 6 a otro padre
task2.Children.Add(task);
```

### Ver también

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Agrega una nueva tarea a la colección de tareas del proyecto en el mismo nivel de esquema de la última tarea.

```csharp
public Task Add()
```

### Valor devuelto

devuelve la nueva instancia añadida de la clase [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Agrega una nueva tarea a la colección de tareas hijas.

```csharp
public Task Add(string taskName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| taskName | Cadena | el nombre de la tarea especificada. |

### Valor devuelto

devuelve la nueva instancia añadida de la clase [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Agrega una nueva tarea recurrente a la colección de tareas hijas.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| taskName | Cadena | el nombre de la tarea especificada. |
| beforeTaskId | Int32 | El ID especificado de una tarea antes del cual se insertará una nueva tarea. |

### Valor devuelto

devuelve una tarea que fue insertada antes de una tarea con el ID especificado.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException se lanza si el ID especificado no es un ID de tarea válido. |

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Inserta una nueva tarea antes de una tarea con el id especificado y en el mismo nivel de esquema.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Los parámetros especificados para la creación de una tarea recurrente. |

### Valor devuelto

devuelve la nueva instancia añadida de la clase [`Task`](../../task/).

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Lanzada si los parámetros especificados son nulos. |
| ArgumentException | Lanzada si los parámetros especificados son inválidos. |

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

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


