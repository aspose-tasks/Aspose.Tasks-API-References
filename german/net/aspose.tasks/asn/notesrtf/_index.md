---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Asn-Feld. Die Textnotizen im RTF-Format. Nur für MPP-Formate unterstützt."
type: docs
weight: 340
url: /de/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

Die Textnotizen im RTF-Format. Nur für MPP-Formate unterstützt.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
```

## Beispiele

Zeigt, wie Ressourcenzuweisungsnotizen abgerufen/gesetzt werden.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// Ressourcenzuweisung erstellen
var assn = project.ResourceAssignments.Add(task, rsc);

// Ressourcenzuweisungsnotizen setzen 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Siehe auch

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


