---
title: "Rsc.RemainingWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. एक कार्य या कार्यों के सेट को पूरा करने के लिए अभी आवश्यक समय"
type: docs
weight: 610
url: /hi/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

किसी कार्य या कार्य समूह को पूरा करने के लिए अभी भी आवश्यक समय।

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## उदाहरण

दिखाता है कि कैसे Rsc.RemainingWork प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


