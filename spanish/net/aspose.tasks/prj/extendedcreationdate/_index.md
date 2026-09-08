---
title: "Prj.ExtendedCreationDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Fecha utilizada para cálculo e informes"
type: docs
weight: 320
url: /es/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Fecha utilizada para el cálculo y la generación de informes.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


