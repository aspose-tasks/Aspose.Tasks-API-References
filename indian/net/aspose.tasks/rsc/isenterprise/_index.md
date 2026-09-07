---
title: "Rsc.IsEnterprise"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। दर्शाता है कि कोई संसाधन एंटरप्राइज़ रिसोर्स पूल से है (true) या स्थानीय रिसोर्स पूल से (false)"
type: docs
weight: 400
url: /hi/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

दर्शाता है कि संसाधन एंटरप्राइज़ संसाधन पूल (सही) से है या स्थानीय संसाधन पूल (गलत) से।

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## उदाहरण

दिखाता है कि Rsc.IsEnterprise प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


