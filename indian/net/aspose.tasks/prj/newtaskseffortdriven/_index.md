---
title: "Prj.NewTasksEffortDriven"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि नई कार्य परिश्रम‑आधारित हैं या नहीं"
type: docs
weight: 560
url: /hi/net/aspose.tasks/prj/newtaskseffortdriven/
---
## Prj.NewTasksEffortDriven field

निर्धारित करता है कि क्या नई कार्यों को प्रयास‑आधारित बनाया गया है।

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEffortDriven;
```

## उदाहरण

दिखाता है कि Prj.NewTasksEffortDriven प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.NewTasksEffortDriven, true);

Console.WriteLine("New Tasks Effort Driven: " + project.Get(Prj.NewTasksEffortDriven));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


