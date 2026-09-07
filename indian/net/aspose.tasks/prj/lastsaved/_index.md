---
title: "Prj.LastSaved"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। वह तिथि जब प्रोजेक्ट आखिरी बार सहेजा गया था। mpp फ़ाइलों में UTC फ़ॉर्मेट में सहेजा गया। DateTime प्रकार"
type: docs
weight: 440
url: /hi/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

परियोजना को अंतिम बार सहेजा गया तिथि। mpp फ़ाइलों में UTC प्रारूप में सहेजा गया। DateTime प्रकार।

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


