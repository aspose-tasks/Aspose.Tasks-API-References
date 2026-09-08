---
title: "Rsc.AccrueAt"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Determina cómo y cuándo se deben cargar o acumular los costos estándar y de horas extra del recurso al costo de una tarea"
type: docs
weight: 10
url: /es/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Determina cómo y cuándo se deben cargar, o acumular, los costos estándar y de horas extra de los recursos al costo de una tarea.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


