---
title: "Asn.Stop"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. वह तिथि जब असाइनमेंट रोक दिया जाता है"
type: docs
weight: 520
url: /hi/net/aspose.tasks/asn/stop/
---
## Asn.Stop field

असाइनमेंट बंद होने की तिथि।

```csharp
public static readonly Key<DateTime, AsnKey> Stop;
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


