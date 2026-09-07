---
title: "Asn.NotesText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। RTF डेटा से निकाला गया नोट्स का साधारण टेक्स्ट।"
type: docs
weight: 350
url: /hi/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

RTF डेटा से निकाले गए नोट्स का साधारण पाठ।

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## उदाहरण

रिसोर्स असाइनमेंट नोट्स को प्राप्त/सेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// रिसोर्स असाइनमेंट बनाएं
var assn = project.ResourceAssignments.Add(task, rsc);

// रिसोर्स असाइनमेंट नोट्स सेट करें 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


