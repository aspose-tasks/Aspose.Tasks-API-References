---
title: "Prj.NewTasksAreManual"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि नए कार्य मैनुअल रूप में बनाए गए हैं"
type: docs
weight: 550
url: /hi/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

निर्धारित करता है कि क्या नई कार्यों को मैन्युअल रूप से बनाया गया है।

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## उदाहरण

दिखाता है कि Prj.NewTasksAreManual प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


