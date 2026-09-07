---
title: "Asn.OvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. एक असाइनमेंट का निर्धारित ओवरटाइम कार्य"
type: docs
weight: 380
url: /hi/net/aspose.tasks/asn/overtimework/
---
## Asn.OvertimeWork field

असाइनमेंट का नियोजित ओवरटाइम कार्य।

```csharp
public static readonly Key<Duration, AsnKey> OvertimeWork;
```

## उदाहरण

दिखाता है कि असाइनमेंट की ओवरटाइम/शेष कार्य/लागत कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// असाइनमेंट ओवरटाइम प्रिंट करें
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


