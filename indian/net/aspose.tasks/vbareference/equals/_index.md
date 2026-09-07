---
title: "VbaReference.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaReference मेथड। यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट VbaReference ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 40
url: /hi/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [`VbaReference`](../) ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public bool Equals(VbaReference other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | VbaReference | यह इंस्टेंस के साथ तुलना करने के लिए निर्दिष्ट [`VbaReference`](../) ऑब्जेक्ट। |

### रिटर्न वैल्यू

यदि यह इंस्टेंस निर्दिष्ट [`VbaReference`](../) ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

दिखाता है कि VBA रेफ़रेंस समानता कैसे जांचें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// रेफ़रेंस की समानता को रेफ़रेंस के नाम के विरुद्ध जांचा जाता है।
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### संबंधित देखें

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [`VbaReference`](../) ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | Object | यह इंस्टेंस के साथ तुलना करने के लिए निर्दिष्ट [`VbaReference`](../) ऑब्जेक्ट। |

### रिटर्न वैल्यू

यदि यह इंस्टेंस निर्दिष्ट [`VbaReference`](../) ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

दिखाता है कि VBA रेफ़रेंस समानता कैसे जांचें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// रेफ़रेंस की समानता को रेफ़रेंस के नाम के विरुद्ध जांचा जाता है।
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### संबंधित देखें

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


