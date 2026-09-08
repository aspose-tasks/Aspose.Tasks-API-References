---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El Active Directory Guid para un recurso"
type: docs
weight: 20
url: /es/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

El GUID de Active Directory para un recurso.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


