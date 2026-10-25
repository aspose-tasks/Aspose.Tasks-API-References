---
title: "Asn.NotesText"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Asn-Feld. Notizen im Klartext, extrahiert aus RTF-Daten."
type: docs
weight: 350
url: /de/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Klartext der Notizen, extrahiert aus RTF-Daten.

```csharp
public static readonly Key<string, AsnKey> NotesText;
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


