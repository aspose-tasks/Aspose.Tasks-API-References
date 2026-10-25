---
title: "Prj.TimescaleFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। वह तिथि जब व्यू में टाइमस्केल समाप्त होता है।"
type: docs
weight: 730
url: /hi/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

व्यू में टाइमस्केल के समाप्त होने की तिथि।

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## उदाहरण

दिखाता है कि Prj.TimescaleFinish प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


