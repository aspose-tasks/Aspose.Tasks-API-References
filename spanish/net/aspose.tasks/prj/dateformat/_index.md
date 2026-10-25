---
title: "Prj.DateFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Formato de fecha de la vista del proyecto"
type: docs
weight: 210
url: /es/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Formato de fecha de la vista del proyecto.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.DateFormat.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


