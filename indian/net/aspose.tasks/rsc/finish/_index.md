---
title: "Rsc.Finish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। वह तिथि जब एक संसाधन को सभी असाइन किए गए कार्यों पर काम पूरा करने के लिए निर्धारित किया जाता है।"
type: docs
weight: 290
url: /hi/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

संसाधन को सभी सौंपे गए कार्यों को पूरा करने के लिए निर्धारित तिथि।

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## उदाहरण

Rsc.Finish प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


