---
title: "Duration.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Duration मेथड। यह इस object के लिए एक हैश कोड मान लौटाता है।"
type: docs
weight: 90
url: /hi/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस duration instance के लिए एक हैश कोड मान लौटाता है।

## उदाहरण

दिखाता है कि duration का हैश कोड कैसे प्राप्त किया जाए।

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// कैलेंडर का हैश कोड समय इकाई प्रकार और duration के प्रारंभिक मान पर आधारित होता है।
// इसलिए अगले हैश कोड समान होते हैं।
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// लेकिन duration 1 और 3 के हैश कोड समान नहीं हैं।
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### संबंधित देखें

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


