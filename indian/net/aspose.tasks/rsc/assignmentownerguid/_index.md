---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। असाइनमेंट मालिक का GUID"
type: docs
weight: 110
url: /hi/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

एक असाइनमेंट मालिक का GUID।

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## उदाहरण

दिखाता है कि Rsc.AssignmentOwnerGuid प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


