---
title: "Prj.CreationDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La fecha y hora en que se creó un proyecto"
type: docs
weight: 130
url: /es/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

La fecha y hora en que se creó un proyecto.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Observaciones

Guardado en formato UTC en archivos mpp. Tipo DateTime.

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


