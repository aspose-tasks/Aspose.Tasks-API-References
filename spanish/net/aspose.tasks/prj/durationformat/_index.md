---
title: "Prj.DurationFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El formato para expresar la duración total"
type: docs
weight: 300
url: /es/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

El formato para expresar la duración total.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


