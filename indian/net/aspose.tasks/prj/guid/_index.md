---
title: "Prj.Guid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। प्रोजेक्ट का GUID"
type: docs
weight: 360
url: /hi/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

परियोजना का GUID।

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## उदाहरण

दिखाता है कि Prj.Guid प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


