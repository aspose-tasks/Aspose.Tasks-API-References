---
title: "Prj.StartDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. एक प्रोजेक्ट की प्रारंभ तिथि"
type: docs
weight: 680
url: /hi/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

परियोजना की प्रारंभ तिथि।

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## उदाहरण

Prj.StartDate प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


