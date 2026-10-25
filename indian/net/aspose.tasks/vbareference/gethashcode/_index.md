---
title: "VbaReference.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaReference मेथड। इस VbaReference के लिए हैश कोड मान लौटाता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

इस [`VbaReference`](../) के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

दिखाता है कि VBA रेफ़रेंस का हैश कोड कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// एक रेफ़रेंस का हैश कोड आंतरिक रेफ़रेंस के GUID का हैश कोड होता है
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### संबंधित देखें

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


