---
title: "Prj.WorkFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. कार्य की अवधि दिखाने के लिए उपयोग किया जाने वाला प्रारूप"
type: docs
weight: 790
url: /hi/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

कार्य की अवधि दिखाने के लिए उपयोग किया जाने वाला फ़ॉर्मेट।

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## उदाहरण

डिफ़ॉल्ट कार्य प्रारूप के साथ अवधि प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// प्रोजेक्ट के डिफ़ॉल्ट कार्य फ़ॉर्मेट के साथ एक कार्य मान बनाएं
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


