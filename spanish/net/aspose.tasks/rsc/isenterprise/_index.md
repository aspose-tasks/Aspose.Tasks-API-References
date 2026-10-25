---
title: "Rsc.IsEnterprise"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Muestra si un recurso proviene del grupo de recursos empresarial (true) o del grupo de recursos local (false)"
type: docs
weight: 400
url: /es/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Muestra si un recurso proviene del grupo de recursos empresarial (true) o del grupo de recursos local (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


