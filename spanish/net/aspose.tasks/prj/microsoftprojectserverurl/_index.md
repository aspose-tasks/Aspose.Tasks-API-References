---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Determina si un proyecto fue creado por un usuario de Project Server en contraposición a un usuario NT"
type: docs
weight: 460
url: /es/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Determina si un proyecto fue creado por un usuario de Project Server en lugar de un usuario NT.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.MicrosoftProjectServerURL.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


