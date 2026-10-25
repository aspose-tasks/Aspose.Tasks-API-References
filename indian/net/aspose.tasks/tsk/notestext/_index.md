---
title: "Tsk.NotesText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। RTF डेटा से निकाला गया नोट्स का साधारण टेक्स्ट"
type: docs
weight: 830
url: /hi/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

RTF डेटा से निकाले गए नोट्स का साधारण पाठ।

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## उदाहरण

दिखाता है कि Tsk.NotesText प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


