---
title: "ResourceAssignment.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। ResourceAssignment क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है"
type: docs
weight: 710
url: /hi/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

[`ResourceAssignment`](../) क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

## उदाहरण

रिसोर्स असाइनमेंट का हैश कोड कैसे प्राप्त करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// असाइनमेंट के हैश कोड प्रिंट करें
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### संबंधित देखें

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


