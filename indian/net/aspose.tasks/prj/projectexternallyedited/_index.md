---
title: "Prj.ProjectExternallyEdited"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि क्या प्रोजेक्ट को बाहरी रूप से संपादित किया गया था"
type: docs
weight: 590
url: /hi/net/aspose.tasks/prj/projectexternallyedited/
---
## Prj.ProjectExternallyEdited field

निर्धारित करता है कि क्या परियोजना को बाहरी रूप से संपादित किया गया था।

```csharp
public static readonly Key<NullableBool, PrjKey> ProjectExternallyEdited;
```

## उदाहरण

दिखाता है कि Prj.ProjectExternallyEdited प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.ProjectExternallyEdited, true);

Console.WriteLine("Project Externally Edited: " + project.Get(Prj.ProjectExternallyEdited));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


