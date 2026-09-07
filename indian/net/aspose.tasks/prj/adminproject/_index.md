---
title: "Prj.AdminProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. निर्धारित करता है कि प्रोजेक्ट एक प्रशासनिक प्रोजेक्ट है या नहीं"
type: docs
weight: 20
url: /hi/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

निर्धारित करता है कि परियोजना एक प्रशासनिक परियोजना है या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## उदाहरण

Prj.AdminProject प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


