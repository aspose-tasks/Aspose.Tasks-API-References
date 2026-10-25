---
title: "Rsc.Uid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी संसाधन का अद्वितीय पहचानकर्ता"
type: docs
weight: 670
url: /hi/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

संसाधन की विशिष्ट पहचानकर्ता।

```csharp
public static readonly Key<int, RscKey> Uid;
```

## उदाहरण

दिखाता है कि Rsc.Uid प्रॉपर्टी को कैसे पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


