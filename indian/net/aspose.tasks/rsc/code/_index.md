---
title: "Rsc.Code"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. किसी संसाधन के बारे में कोड या अन्य जानकारी"
type: docs
weight: 210
url: /hi/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

संसाधन के बारे में कोड या अन्य जानकारी।

```csharp
public static readonly Key<string, RscKey> Code;
```

## उदाहरण

दिखाता है कि Rsc.Code प्रॉपर्टी को कैसे पढ़ें/लिखें.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


