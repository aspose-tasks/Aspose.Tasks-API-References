---
title: "Prj.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El nombre del proyecto"
type: docs
weight: 540
url: /es/net/aspose.tasks/prj/name/
---
## Prj.Name field

El nombre del proyecto.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Ejemplos

Muestra cómo leer/escribir el nombre del proyecto.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


