---
title: "Rsc.PeakUnits"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन के लिए किसी भी समय सभी कार्यों में असाइन किए गए अधिकतम असाइनमेंट यूनिट"
type: docs
weight: 540
url: /hi/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

संसाधन को सौंपे गए सभी कार्यों के लिए किसी भी समय बिंदु पर संसाधन की अधिकतम असाइनमेंट इकाई।

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## उदाहरण

दिखाता है कि कैसे Rsc.PeakUnits प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


