---
title: "Prj.EarnedValueMethod"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। अर्जित मूल्य की गणना के लिए डिफ़ॉल्ट विधि"
type: docs
weight: 310
url: /hi/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

अर्जित मूल्य की गणना के लिए डिफ़ॉल्ट विधि।

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## उदाहरण

दिखाता है कि Prj.EarnedValueMethod प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


