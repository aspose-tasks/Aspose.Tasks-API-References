---
title: Rsc.NotesText
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Notes plain text extracted from RTF data
type: docs
weight: 480
url: /net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Notes' plain text extracted from RTF data.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Examples

Shows how to read/write Rsc.NotesText property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


