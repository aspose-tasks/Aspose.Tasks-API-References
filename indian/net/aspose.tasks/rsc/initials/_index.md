---
title: "Rsc.Initials"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। एक संसाधन के प्रारंभिक अक्षर।"
type: docs
weight: 370
url: /hi/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

संसाधन के प्रारंभिक अक्षर।

```csharp
public static readonly Key<string, RscKey> Initials;
```

## उदाहरण

Rsc.Initials प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


