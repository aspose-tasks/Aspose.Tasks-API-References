---
title: "Prj.SplitsInProgressTasks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि प्रगति में चल रहे कार्यों को विभाजित किया जा सकता है या नहीं"
type: docs
weight: 650
url: /hi/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

निर्धारित करता है कि क्या प्रगति में चल रहे कार्यों को विभाजित किया जा सकता है।

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## उदाहरण

दिखाता है कि Prj.SplitsInProgressTasks प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


