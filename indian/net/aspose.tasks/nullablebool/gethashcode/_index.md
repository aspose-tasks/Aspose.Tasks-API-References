---
title: "NullableBool.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "NullableBool मेथड। यह NullableBool क्लास के इंस्टेंस के लिए एक हैश कोड मान लौटाता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

[`NullableBool`](../) क्लास के इंस्टेंस के लिए एक हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

दिखाता है कि कैसे &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode मेथड के साथ काम किया जाए।

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// बूल्स का हैश कोड 'IsDefined' और 'Value' प्रॉपर्टीज़ पर आधारित होता है
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### संबंधित देखें

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


