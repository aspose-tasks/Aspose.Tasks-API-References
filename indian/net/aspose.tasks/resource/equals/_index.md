---
title: "Resource.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource मेथड। यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस Resource क्लास के निर्दिष्ट इंस्टेंस के बराबर है या नहीं।"
type: docs
weight: 820
url: /hi/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट [`Resource`](../) क्लास के इंस्टेंस के बराबर है या नहीं।

```csharp
public bool Equals(Resource other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | Resource | यह इंस्टेंस के साथ तुलना करने के लिए निर्दिष्ट [`Resource`](../) क्लास का इंस्टेंस। |

### रिटर्न वैल्यू

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## उदाहरण

संसाधन समानता की जाँच कैसे करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### संबंधित देखें

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
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

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## उदाहरण

संसाधन समानता की जाँच कैसे करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### संबंधित देखें

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


