---
title: "Prj.Guid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El GUID del proyecto"
type: docs
weight: 360
url: /es/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

El GUID del proyecto.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


