---
title: "Asn.PercentWorkComplete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. एक असाइनमेंट पर पूर्ण किए गए कार्य की मात्रा"
type: docs
weight: 400
url: /hi/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

एक असाइनमेंट पर पूर्ण किए गए कार्य की मात्रा।

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## उदाहरण

असाइनमेंट की पूर्ण कार्य प्रतिशत को कैसे पढ़ें दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// असाइनमेंट की प्रतिशत पूर्णता प्रिंट करें
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


