---
title: "Filter.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Filter method. यह दर्शाने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline वस्तु के बराबर है या नहीं।"
type: docs
weight: 100
url: /hi/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public bool Equals(Filter other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | Filter | इस उदाहरण से तुलना करने के लिए निर्दिष्ट AssignmentBaseline वस्तु। |

### रिटर्न वैल्यू

यदि यह उदाहरण निर्दिष्ट AssignmentBaseline वस्तु के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

फ़िल्टर समानता की जाँच कैसे करें दिखाता है.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// फ़िल्टरों की समानता को फ़िल्टर के UID के विरुद्ध जाँच किया जाता है.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### संबंधित देखें

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | इस उदाहरण से तुलना करने के लिए निर्दिष्ट AssignmentBaseline वस्तु। |

### रिटर्न वैल्यू

यदि यह उदाहरण निर्दिष्ट AssignmentBaseline वस्तु के बराबर है तो true लौटाता है; अन्यथा false।

## उदाहरण

फ़िल्टर समानता की जाँच कैसे करें दिखाता है.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// फ़िल्टरों की समानता को फ़िल्टर के UID के विरुद्ध जाँच किया जाता है.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### संबंधित देखें

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


