---
title: "Prj.NewTaskStartDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El tipo de fecha de inicio predeterminada para nuevas tareas"
type: docs
weight: 580
url: /es/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

El tipo de fecha de inicio predeterminada para tareas nuevas.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Ejemplos

Muestra cómo establecer atributos para nuevas tareas.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


