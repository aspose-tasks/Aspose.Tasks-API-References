---
title: "Resource.Delete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource मेथड। प्रोजेक्ट से एक रिसोर्स और उसकी असाइनमेंट्स को हटाता है"
type: docs
weight: 810
url: /hi/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

प्रोजेक्ट से एक संसाधन और उसकी असाइनमेंट्स को हटाता है।

```csharp
public void Delete()
```

## उदाहरण

रिसोर्स को डिलीट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// रिसोर्स को हटाएँ
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### संबंधित देखें

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


