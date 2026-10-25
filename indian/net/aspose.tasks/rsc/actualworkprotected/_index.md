---
title: "Rsc.ActualWorkProtected"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। वह कार्य मात्रा जिसके द्वारा वास्तविक कार्य संरक्षित रहता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

वह कार्य मात्रा जिसके माध्यम से वास्तविक कार्य संरक्षित रहता है।

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## उदाहरण

दिखाता है कि Rsc.ActualWorkProtected प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


