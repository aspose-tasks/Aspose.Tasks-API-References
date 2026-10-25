---
title: "Asn.NotesText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Texto plano de notas extraído de datos RTF"
type: docs
weight: 350
url: /es/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Texto plano de las notas extraído de los datos RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## Ejemplos

Muestra cómo obtener/establecer notas de asignación de recursos.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// crear asignación de recursos
var assn = project.ResourceAssignments.Add(task, rsc);

// establecer notas de asignación de recursos 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


