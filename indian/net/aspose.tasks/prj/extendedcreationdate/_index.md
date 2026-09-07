---
title: "Prj.ExtendedCreationDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड. गणना और रिपोर्टिंग के लिए उपयोग की गई तिथि"
type: docs
weight: 320
url: /hi/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

गणना और रिपोर्टिंग के लिए प्रयुक्त तिथि।

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## उदाहरण

दिखाता है कि Prj.ExtendedCreationDate प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


