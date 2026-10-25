---
title: "Prj.TimescaleStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। वह तिथि जब व्यू में टाइमस्केल शुरू होता है।"
type: docs
weight: 740
url: /hi/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

व्यू में टाइमस्केल के शुरू होने की तिथि।

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## उदाहरण

दिखाता है कि टाइमस्केल प्रारंभ तिथि को कैसे सेट करें ताकि व्यू की प्रारंभ तिथि को समायोजित किया जा सके।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


