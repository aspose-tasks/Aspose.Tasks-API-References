---
title: "Prj.TimescaleFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La fecha en que finaliza la escala de tiempo en la vista."
type: docs
weight: 730
url: /es/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

La fecha en que la escala de tiempo en la vista finaliza.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


