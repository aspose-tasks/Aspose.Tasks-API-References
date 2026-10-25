---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModuleAttribute मेथड। इस VbaModuleAttribute के लिए हैश कोड मान लौटाता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

इस [`VbaModuleAttribute`](../) के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

दिखाता है कि VBA मॉड्यूल एट्रिब्यूट का हैश कोड कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// VBA मॉड्यूल एट्रिब्यूट्स के हैश कोड प्रिंट करें
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### संबंधित देखें

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


