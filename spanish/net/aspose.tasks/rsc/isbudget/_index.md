---
title: "Rsc.IsBudget"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. Determina si un recurso de material de trabajo o de costo es un recurso de presupuesto"
type: docs
weight: 380
url: /es/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Determina si un recurso de trabajo, material o costo es un recurso presupuestario.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


