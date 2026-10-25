---
title: "Prj.CurrentDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La fecha del sistema"
type: docs
weight: 190
url: /es/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

La fecha del sistema.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.CurrentDate.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


