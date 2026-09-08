---
title: "Prj.Manager"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El responsable de un proyecto"
type: docs
weight: 450
url: /es/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

El responsable del proyecto.

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.Manager.

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


