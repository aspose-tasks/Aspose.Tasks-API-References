---
title: "Enumeración TaskStartDateType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.TaskStartDateType enum. Especifica el tipo de la fecha de inicio de una tarea."
type: docs
weight: 2450
url: /es/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Especifica el tipo de la fecha de inicio de una tarea.

```csharp
public enum TaskStartDateType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | El valor del campo no estaba definido en el archivo de proyecto original. |
| ProjectStartDate | `0` | Fecha de inicio del proyecto |
| CurrentDate | `1` | Fecha actual |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo establecer la fecha de inicio predeterminada de la tarea como 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


