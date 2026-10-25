---
title: "Rsc.ActualOvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। कार्यों को सौंपे गए संसाधन द्वारा पहले से किए गए ओवरटाइम कार्य की वास्तविक मात्रा"
type: docs
weight: 50
url: /hi/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

कार्य सौंपे गए संसाधन द्वारा पहले से किए गए ओवरटाइम कार्य की वास्तविक मात्रा।

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## उदाहरण

दिखाता है कि Rsc.ActualOvertimeWork प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


