---
title: "Tsk.NotesRTF"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. RTF स्वरूप में पाठ नोट्स। केवल MPP स्वरूपों के लिए समर्थित"
type: docs
weight: 820
url: /hi/net/aspose.tasks/tsk/notesrtf/
---
## Tsk.NotesRTF field

RTF प्रारूप में पाठ नोट्स। केवल MPP प्रारूपों के लिए समर्थित।

```csharp
public static readonly Key<string, TaskKey> NotesRTF;
```

## उदाहरण

दिखाता है कि कैसे Tsk.NotesRTF प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

            var task = project.RootTask.Children.Add("Task");

            const string rtf = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            task.Set(Tsk.NotesRTF, rtf);

            Console.WriteLine("Notes RTF: " + task.Get(Tsk.NotesRTF));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


