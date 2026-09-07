---
title: "Rsc.ActualWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। वह कार्य मात्रा जो पहले ही कार्यों को असाइन किए गए संसाधन द्वारा पूरी हो चुकी है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

कार्य सौंपे गए संसाधन द्वारा पहले से किए गए कार्य की मात्रा।

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## उदाहरण

दिखाता है कि कैसे Rsc.ActualWork प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


