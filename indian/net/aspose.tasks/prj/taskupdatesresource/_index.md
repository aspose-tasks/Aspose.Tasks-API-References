---
title: "Prj.TaskUpdatesResource"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि कार्यों में अपडेट संसाधनों को अपडेट करते हैं या नहीं"
type: docs
weight: 710
url: /hi/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

निर्धारित करता है कि क्या कार्यों में अपडेट संसाधनों को अपडेट करते हैं।

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## उदाहरण

दिखाता है कि Prj.TaskUpdatesResource प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


