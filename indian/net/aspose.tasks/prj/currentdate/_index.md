---
title: "Prj.CurrentDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। सिस्टम की तिथि"
type: docs
weight: 190
url: /hi/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

सिस्टम तिथि।

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## उदाहरण

दिखाता है कि Prj.CurrentDate प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


