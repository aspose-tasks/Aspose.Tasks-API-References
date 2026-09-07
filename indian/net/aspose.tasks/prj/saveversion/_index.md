---
title: "Prj.SaveVersion"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. Microsoft Office Project का वह संस्करण जिससे प्रोजेक्ट फ़ाइल सहेजी गई थी"
type: docs
weight: 620
url: /hi/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

Microsoft Office Project का वह संस्करण जिससे परियोजना फ़ाइल सहेजी गई थी।

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## उदाहरण

दिखाता है कि प्रोजेक्ट के सहेजने का संस्करण और सहेजने की तिथि कैसे जांचें।

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// प्रोजेक्ट संस्करण दिखाएँ
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


