---
title: "Rsc.Phonetics"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. संसाधन नाम की ध्वन्यात्मक वर्तनी। केवल जापानी के उपयोग के लिए।"
type: docs
weight: 560
url: /hi/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

संसाधन नाम की ध्वन्यात्मक वर्तनी। केवल जापानी के उपयोग के लिए।

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## उदाहरण

दिखाता है कि कैसे Rsc.Phonetics प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


