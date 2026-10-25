---
title: "Prj.RemoveFileProperties"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si todas las propiedades de archivo se eliminarán al guardar"
type: docs
weight: 600
url: /es/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Determina si todas las propiedades del archivo se eliminarán al guardar.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


