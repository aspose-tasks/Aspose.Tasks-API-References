---
title: "Prj.ShowProjectSummaryTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si se muestra información resumida de todo el proyecto en una sola fila con su propia barra de tarea resumen en la parte superior de la vista de diagrama de Gantt"
type: docs
weight: 640
url: /es/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Determina si se muestra la información resumida de todo el proyecto en una sola fila con su propia barra de tarea resumen en la parte superior de la vista de diagrama de Gantt.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.ShowProjectSummaryTask.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


