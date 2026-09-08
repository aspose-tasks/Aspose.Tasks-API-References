---
title: "Rsc.MaterialLabel"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La unidad de medida para el recurso material"
type: docs
weight: 440
url: /es/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

La unidad de medida del recurso material.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


