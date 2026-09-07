---
title: "ResourceAssignment.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ResourceAssignment क्लास के इंस्टेंस के बराबर है या नहीं"
type: docs
weight: 690
url: /hi/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [`ResourceAssignment`](../) क्लास के इंस्टेंस के बराबर है या नहीं।

```csharp
public bool Equals(ResourceAssignment other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | ResourceAssignment | निर्दिष्ट [`ResourceAssignment`](../) क्लास का इंस्टेंस जिसे इस इंस्टेंस से तुलना की जाती है। |

### रिटर्न वैल्यू

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## उदाहरण

दिखाता है कि कैसे रिसोर्स असाइनमेंट की समानता जाँचें।

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### संबंधित देखें

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस इंस्टेंस के साथ तुलना करने के लिए वस्तु। |

### रिटर्न वैल्यू

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## उदाहरण

दिखाता है कि कैसे रिसोर्स असाइनमेंट की समानता जाँचें।

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### संबंधित देखें

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


