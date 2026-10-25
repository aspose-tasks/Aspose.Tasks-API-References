---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड. निर्धारित करता है कि नई संसाधन या कार्य स्वचालित रूप से संसाधन या कार्य पूल में जोड़े जाएँ"
type: docs
weight: 50
url: /hi/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

निर्धारित करता है कि नए संसाधन या कार्य स्वचालित रूप से संसाधन या कार्य पूल में जोड़े गए हैं या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## उदाहरण

दिखाता है कि Prj.AutoAddNewResourcesAndTasks प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


