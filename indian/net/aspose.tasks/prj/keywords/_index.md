---
title: "Prj.Keywords"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट के कीवर्ड्स"
type: docs
weight: 410
url: /hi/net/aspose.tasks/prj/keywords/
---
## Prj.Keywords field

परियोजना के कीवर्ड।

```csharp
public static readonly Key<string, PrjKey> Keywords;
```

## उदाहरण

दिखाता है कि परियोजना मेटा जानकारी कैसे सेट करें।

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// परियोजना जानकारी सेट करें
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


