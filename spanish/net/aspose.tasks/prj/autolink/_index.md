---
title: "Prj.Autolink"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si las tareas insertadas o movidas se enlazan automáticamente"
type: docs
weight: 70
url: /es/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Determina si las tareas insertadas o movidas se enlazan automáticamente.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


