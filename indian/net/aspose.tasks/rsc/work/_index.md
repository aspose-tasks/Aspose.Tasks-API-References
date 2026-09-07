---
title: "Rsc.Work"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। किसी कार्य पर संसाधन के लिए निर्धारित कुल समय"
type: docs
weight: 690
url: /hi/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

किसी कार्य में संसाधन के लिए निर्धारित कुल समय।

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## उदाहरण

दिखाता है कि Rsc.Work प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


