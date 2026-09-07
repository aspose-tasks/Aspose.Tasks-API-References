---
title: "Filter.CompareTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Filter method. इस उदाहरण की तुलना निर्दिष्ट Filter वर्ग के उदाहरण से करता है और उनके सापेक्ष क्रम का संकेत लौटाता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

इस उदाहरण की तुलना निर्दिष्ट [`Filter`](../) वर्ग के उदाहरण से करता है और उनके सापेक्ष क्रम का संकेत लौटाता है।

```csharp
public int CompareTo(Filter other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | Filter | इस वस्तु से तुलना करने के लिए निर्दिष्ट [`Filter`](../) वर्ग का उदाहरण। |

### रिटर्न वैल्यू

उनके सापेक्ष क्रम का एक संकेत।

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


