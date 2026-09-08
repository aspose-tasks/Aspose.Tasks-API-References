---
title: "Prj.LastPrinted"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Última hora de impresión del proyecto. Guardado en formato UTC en archivos mpp. Tipo DateTime."
type: docs
weight: 430
url: /es/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Última hora de impresión del proyecto. Guardada en formato UTC en archivos mpp. Tipo DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


