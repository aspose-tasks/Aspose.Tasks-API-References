---
title: "Rsc.NotesText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Texto plano de notas extraído de datos RTF"
type: docs
weight: 480
url: /es/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Texto plano de las notas extraído de los datos RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


