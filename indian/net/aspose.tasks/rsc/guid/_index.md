---
title: "Rsc.Guid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड. संसाधन के लिए उत्पन्न अद्वितीय पहचान कोड शामिल करता है"
type: docs
weight: 310
url: /hi/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

संसाधन के लिए उत्पन्न अद्वितीय पहचान कोड शामिल करता है।

```csharp
public static readonly Key<string, RscKey> Guid;
```

## उदाहरण

दिखाता है कि कैसे Rsc.Guid प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


