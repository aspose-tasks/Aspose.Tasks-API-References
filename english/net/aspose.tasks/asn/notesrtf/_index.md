---
title: Asn.NotesRTF
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The text notes in RTF format. Supported for MPP formats only
type: docs
weight: 340
url: /net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

The text notes in RTF format. Supported for MPP formats only.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
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


