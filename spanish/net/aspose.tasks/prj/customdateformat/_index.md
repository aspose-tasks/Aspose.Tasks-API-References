---
title: "Prj.CustomDateFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Formato de fecha personalizado de la vista del proyecto. Se usa para formatear fechas cuando la propiedad DateFormat está establecida en Custom"
type: docs
weight: 200
url: /es/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Formato de fecha personalizado de la vista del proyecto. Se usa para formatear fechas cuando la propiedad [`DateFormat`](../dateformat/) está establecida en Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


