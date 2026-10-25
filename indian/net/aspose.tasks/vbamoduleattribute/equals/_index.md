---
title: "VbaModuleAttribute.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModuleAttribute मेथड। यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट VbaModuleAttribute ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 30
url: /hi/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [`VbaModuleAttribute`](../) ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public bool Equals(VbaModuleAttribute other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | VbaModuleAttribute | यह इंस्टेंस के साथ तुलना करने के लिए निर्दिष्ट [`VbaModuleAttribute`](../) ऑब्जेक्ट। |

### रिटर्न वैल्यू

यदि यह इंस्टेंस निर्दिष्ट [`VbaModuleAttribute`](../) ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

दिखाता है कि VBA मॉड्यूल एट्रिब्यूट्स की समानता कैसे जांचें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### संबंधित देखें

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [`VbaModuleAttribute`](../) ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | Object | यह इंस्टेंस के साथ तुलना करने के लिए निर्दिष्ट [`VbaModuleAttribute`](../) ऑब्जेक्ट। |

### रिटर्न वैल्यू

यदि यह इंस्टेंस निर्दिष्ट [`VbaModuleAttribute`](../) ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

दिखाता है कि VBA मॉड्यूल एट्रिब्यूट्स की समानता कैसे जांचें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### संबंधित देखें

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


