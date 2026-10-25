---
title: "Prj.TimescaleStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La fecha en que comienza la escala de tiempo en la vista."
type: docs
weight: 740
url: /es/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

La fecha en que la escala de tiempo en la vista comienza.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Ejemplos

Muestra cómo establecer la fecha de inicio de la escala de tiempo para ajustar la fecha en que la vista debe comenzar.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


