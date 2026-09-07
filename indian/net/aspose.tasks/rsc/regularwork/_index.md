---
title: "Rsc.RegularWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। संसाधन द्वारा किए जाने वाले गैर‑ओवरटाइम कार्य की कुल मात्रा"
type: docs
weight: 570
url: /hi/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

संसाधन द्वारा किए जाने वाले गैर-ओवरटाइम कार्य की कुल मात्रा निर्धारित।

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## उदाहरण

दिखाता है कि Rsc.RegularWork प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


