---
title: "Prj.Name"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट का नाम"
type: docs
weight: 540
url: /hi/net/aspose.tasks/prj/name/
---
## Prj.Name field

परियोजना का नाम।

```csharp
public static readonly Key<string, PrjKey> Name;
```

## उदाहरण

परियोजना नाम को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


