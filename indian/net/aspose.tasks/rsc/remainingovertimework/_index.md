---
title: "Rsc.RemainingOvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. शेष निर्धारित ओवरटाइम की मात्रा"
type: docs
weight: 600
url: /hi/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

शेष निर्धारित ओवरटाइम की मात्रा।

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## उदाहरण

दिखाता है कि कैसे Rsc.RemainingOvertimeWork प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


