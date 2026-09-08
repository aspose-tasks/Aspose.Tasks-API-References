---
title: "Prj.StatusDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. la fecha de estado para mostrar el progreso o calcular los totales de valor ganado. La fecha de estado es la misma que la fecha actual a menos que se especifique una fecha de estado diferente"
type: docs
weight: 690
url: /es/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

la fecha de estado para mostrar el progreso o calcular los totales de valor ganado. La fecha de estado es la misma que la fecha actual (fecha de hoy) a menos que se especifique una fecha de estado diferente.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


