---
title: "Rsc.NotesText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। नोट्स का साधारण पाठ जो RTF डेटा से निकाला गया है"
type: docs
weight: 480
url: /hi/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

RTF डेटा से निकाले गए नोट्स का साधारण पाठ।

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## उदाहरण

दिखाता है कि कैसे Rsc.NotesText प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


