---
title: "Project.CalculationMode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Project. Obtiene o establece el modo de cálculo de un proyecto. Puede ser uno de los valores de la enumeración CalculationMode"
type: docs
weight: 110
url: /es/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Obtiene o establece el modo de cálculo de un proyecto. Puede ser uno de los valores de la enumeración `CalculationMode`.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Ejemplos

Muestra cómo usar el modo de cálculo del proyecto.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Establezca la fecha de inicio del proyecto y añada nuevas tareas
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Las propiedades necesarias se establecen en modo manual
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Cuando vinculamos dos tareas juntas sus fechas no se recalculan en modo manual
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// El inicio de la Tarea 2 no ha sido cambiado
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Ver también

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


