---
title: "Rsc.NotesRTF"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. RTF फ़ॉर्मेट में टेक्स्ट नोट्स। केवल MPP फ़ॉर्मेट्स के लिए समर्थित।"
type: docs
weight: 470
url: /hi/net/aspose.tasks/rsc/notesrtf/
---
## Rsc.NotesRTF field

RTF प्रारूप में पाठ नोट्स। केवल MPP प्रारूपों के लिए समर्थित।

```csharp
public static readonly Key<string, RscKey> NotesRTF;
```

## उदाहरण

दिखाता है कि कैसे Rsc.NotesRTF प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

            var resource = project.Resources.Add("Resource");

            const string RTF = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            resource.Set(Rsc.NotesRTF, RTF);

            Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
            Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


