---
title: "Prj.DefaultFinishTime"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड. नए कार्यों का डिफ़ॉल्ट समाप्ति समय"
type: docs
weight: 230
url: /hi/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

नए कार्यों का डिफ़ॉल्ट समाप्ति समय।

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## उदाहरण

दिखाता है कि Prj.DefaultFinishTime प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


