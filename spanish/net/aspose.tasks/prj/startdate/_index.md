---
title: "Prj.StartDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La fecha de inicio de un proyecto"
type: docs
weight: 680
url: /es/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

La fecha de inicio de un proyecto.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


