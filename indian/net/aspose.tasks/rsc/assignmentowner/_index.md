---
title: "Rsc.AssignmentOwner"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। असाइनमेंट मालिक का नाम"
type: docs
weight: 100
url: /hi/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

एक असाइनमेंट मालिक का नाम।

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## उदाहरण

दिखाता है कि कैसे Rsc.AssignmentOwner प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


