---
title: "Filter.op_Equality"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Filter method. यह दर्शाने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट वस्तु के बराबर है या नहीं।"
type: docs
weight: 120
url: /hi/net/aspose.tasks/filter/op_equality/
---
## Filter Equality operator

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public static bool operator ==(Filter a, Filter b)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एक | Filter | पहला फ़िल्टर. |
| b | Filter | दूसरा फ़िल्टर. |

### रिटर्न वैल्यू

एक मान जो दर्शाता है कि यह उदाहरण निर्दिष्ट वस्तु के बराबर है या नहीं।

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


