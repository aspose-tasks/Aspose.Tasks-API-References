---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। दिखाता है कि वर्तमान संसाधन एक टीम संसाधन है या नहीं"
type: docs
weight: 430
url: /hi/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

दर्शाता है कि वर्तमान संसाधन टीम संसाधन है या नहीं।

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## उदाहरण

दिखाता है कि कैसे पढ़ें/लिखें Rsc.IsTeamAssignmentPool प्रॉपर्टी।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


