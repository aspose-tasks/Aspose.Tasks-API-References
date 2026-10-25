---
title: "क्लास फ़िल्टर"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Filter क्लास। प्रोजेक्ट में एक फ़िल्टर का प्रतिनिधित्व करता है।"
type: docs
weight: 600
url: /hi/net/aspose.tasks/filter/
---
## Filter class

प्रोजेक्ट में एक फ़िल्टर का प्रतिनिधित्व करता है।

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Filter](filter/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | टास्क या रिसोर्सेज़ को MSP व्यू में प्रदर्शित होने के लिए आवश्यक मानदंड प्राप्त करता है या सेट करता है। |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | फ़िल्टर का प्रकार प्राप्त करता है। |
| [Index](../../aspose.tasks/filter/index/) { get; } | `Filter` ऑब्जेक्ट का इंडेक्स प्राप्त करता है जो Filters कंटेनिंग ऑब्जेक्ट में है। |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | फ़िल्टर ऑब्जेक्ट का नाम प्राप्त करता है या सेट करता है। |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | प्रोजेक्ट फ़िल्टर नाम को रिबन के व्यू टैब पर फ़िल्टर ड्रॉप-डाउन सूची में दिखाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | फ़िल्टर के लिए संबंधित सारांश पंक्तियों को प्रदर्शित किया जाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | फ़िल्टर की अद्वितीय पहचानकर्ता प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | इस उदाहरण की निर्दिष्ट `Filter` क्लास के उदाहरण से तुलना करता है और उनके सापेक्ष क्रम का संकेत लौटाता है। |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं। |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट AssignmentBaseline ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | फ़िल्टर के लिए हैश कोड मान लौटाता है। |
| [operator ==](../../aspose.tasks/filter/op_equality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं। |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं। |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं। |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं। |

## उदाहरण

फ़िल्टर के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// संसाधन फ़िल्टर जांचें
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


