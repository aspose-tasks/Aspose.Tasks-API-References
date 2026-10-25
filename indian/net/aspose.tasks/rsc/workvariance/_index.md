---
title: "Rsc.WorkVariance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन के बेसलाइन कार्य और वर्तमान में निर्धारित कार्य के बीच का अंतर"
type: docs
weight: 710
url: /hi/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

संसाधन के बेसलाइन कार्य और वर्तमान में निर्धारित कार्य के बीच अंतर।

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## उदाहरण

दिखाता है कि कैसे संसाधन कार्य वैरिएंस पढ़ें।

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


