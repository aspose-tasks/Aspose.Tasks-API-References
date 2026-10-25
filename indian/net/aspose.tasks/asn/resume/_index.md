---
title: "Asn.Resume"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। वह तिथि जब असाइनमेंट फिर से शुरू किया जाता है।"
type: docs
weight: 490
url: /hi/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

असाइनमेंट पुनः शुरू होने की तिथि।

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## उदाहरण

दिखाता है कि कैसे असाइनमेंट की रोक/पुनः प्रारंभ तिथियों को पढ़ें।

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// संसाधन असाइनमेंट की रोक और पुनः प्रारंभ तिथियों को प्रिंट करें
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


