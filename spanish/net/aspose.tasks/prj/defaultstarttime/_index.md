---
title: "Prj.DefaultStartTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La hora de inicio predeterminada de nuevas tareas"
type: docs
weight: 270
url: /es/net/aspose.tasks/prj/defaultstarttime/
---
## Prj.DefaultStartTime field

La hora de inicio predeterminada de las tareas nuevas.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultStartTime;
```

## Ejemplos

Muestra cómo leer las propiedades predeterminadas del proyecto.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Establecer propiedades predeterminadas
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Mostrar propiedades predeterminadas
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


