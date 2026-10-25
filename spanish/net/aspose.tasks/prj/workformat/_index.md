---
title: "Prj.WorkFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El formato usado para mostrar la duración de la tarea"
type: docs
weight: 790
url: /es/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

El formato usado para mostrar la duración de la tarea.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Ejemplos

Muestra cómo obtener una duración con el formato de trabajo predeterminado.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// crear un valor de trabajo con el formato de trabajo predeterminado del proyecto
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


