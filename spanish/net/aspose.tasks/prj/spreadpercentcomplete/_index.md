---
title: "Prj.SpreadPercentComplete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si un porcentaje completado se distribuye a la fecha de estado"
type: docs
weight: 670
url: /es/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

Determina si el porcentaje de completado se distribuye hasta la fecha de estado.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.SpreadPercentComplete.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


