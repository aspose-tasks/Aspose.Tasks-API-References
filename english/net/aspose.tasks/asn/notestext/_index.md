---
title: Asn.NotesText
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. Notes plain text extracted from RTF data
type: docs
weight: 350
url: /net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Notes' plain text extracted from RTF data.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## Examples

Shows how to get/set resource assignment notes.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// create resource assignment
var assn = project.ResourceAssignments.Add(task, rsc);

// set resource assignment notes 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


