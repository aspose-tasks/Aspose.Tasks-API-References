---
title: "Asn.NotesRTF"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. Las notas de texto en formato RTF. Compatible solo con formatos MPP"
type: docs
weight: 340
url: /es/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

Las notas de texto en formato RTF. Compatibles solo con formatos MPP.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
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


