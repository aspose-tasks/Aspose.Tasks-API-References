---
title: "Resource.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource मेथड। Resource क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है"
type: docs
weight: 840
url: /hi/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

इंस्टेंस के लिए हैश कोड मान लौटाता है [`Resource`](../) क्लास।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

रिसोर्स का हैश कोड प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// रिसोर्स का हैश कोड रिसोर्स UID के बराबर है
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### संबंधित देखें

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


