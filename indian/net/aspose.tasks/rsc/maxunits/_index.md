---
title: "Rsc.MaxUnits"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. अधिकतम इकाइयों की संख्या जो अधिकतम क्षमता को दर्शाती है, जिसके लिए एक संसाधन वर्तमान समय अवधि में किसी भी कार्य को पूरा करने के लिए उपलब्ध है।"
type: docs
weight: 450
url: /hi/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

वर्तमान समय अवधि में संसाधन द्वारा किसी भी कार्य को पूरा करने के लिए उपलब्ध अधिकतम क्षमता को दर्शाने वाली अधिकतम इकाइयों की संख्या।

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## उदाहरण

दिखाता है कि कैसे Rsc.MaxUnits प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


