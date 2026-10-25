---
title: "Rsc.StandardRate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. किसी संसाधन द्वारा किए गए नियमित गैर‑ओवरटाइम कार्य के लिए वेतन दर"
type: docs
weight: 620
url: /hi/net/aspose.tasks/rsc/standardrate/
---
## Rsc.StandardRate field

संसाधन द्वारा किए गए नियमित, गैर-ओवरटाइम कार्य के लिए वेतन दर।

```csharp
public static readonly Key<decimal, RscKey> StandardRate;
```

## उदाहरण

दिखाता है कि कैसे संसाधन दरें और समूहों के साथ काम करें।

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// रिसोर्स जोड़ें और कुछ प्रॉपर्टीज़ सेट करें
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


