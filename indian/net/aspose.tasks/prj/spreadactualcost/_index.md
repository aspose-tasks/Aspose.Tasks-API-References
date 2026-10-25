---
title: "Prj.SpreadActualCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. निर्धारित करता है कि वास्तविक लागतें स्थिति तिथि तक फैलायी जाती हैं या नहीं"
type: docs
weight: 660
url: /hi/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

निर्धारित करता है कि क्या वास्तविक लागतें स्थिति तिथि तक वितरित की जाती हैं।

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## उदाहरण

Prj.SpreadActualCost प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


