---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. RTF प्रारूप में टेक्स्ट नोट्स। केवल MPP फ़ॉर्मेट के लिए समर्थित"
type: docs
weight: 340
url: /hi/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

RTF प्रारूप में पाठ नोट्स। केवल MPP प्रारूपों के लिए समर्थित।

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
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


