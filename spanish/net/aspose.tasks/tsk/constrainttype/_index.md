---
title: "Tsk.ConstraintType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Proporciona opciones para el tipo de restricción que se puede aplicar al programar una tarea"
type: docs
weight: 210
url: /es/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

Proporciona opciones para el tipo de restricción que se puede aplicar al programar una tarea.

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
```

## Ejemplos

Muestra cómo obtener/establecer una restricción para una tarea.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Establecer restricción Tan Tarde Como Sea Posible para la tarea con Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


