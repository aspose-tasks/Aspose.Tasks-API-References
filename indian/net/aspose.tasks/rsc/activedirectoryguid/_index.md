---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. एक संसाधन के लिए Active Directory Guid"
type: docs
weight: 20
url: /hi/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

रिसोर्स के लिए Active Directory Guid।

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## उदाहरण

दिखाता है कि कैसे Rsc.ActiveDirectoryGuid प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


