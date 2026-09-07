---
title: "क्लास FilterCriteria"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.FilterCriteria क्लास। उन मानदंडों को परिभाषित करता है जिन्हें कार्यों या संसाधनों को MSP दृश्य में प्रदर्शित होने के लिए पूरा करना चाहिए"
type: docs
weight: 630
url: /hi/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

MSP दृश्य में प्रदर्शित होने के लिए कार्यों या संसाधनों को पूरा करनी वाली मानदंडों को परिभाषित करता है।

```csharp
public class FilterCriteria
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | चाइल्ड `FilterCriteria` पंक्तियों की सूची प्राप्त करता है। यदि फ़िल्टर में एक से अधिक मानदंड पंक्तियाँ हैं तो AND ऑपरेटर का प्रभाव यह है कि दोनों पंक्तियों के मानदंडों को पूरा करना आवश्यक है ताकि कार्य या संसाधन इस फ़िल्टर के परिणामस्वरूप प्रदर्शित हो सके। OR ऑपरेटर का प्रभाव यह है कि एक या दूसरी पंक्ति का मानदंड पूरा होना चाहिए। |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | एक [`Field`](./field/) को प्राप्त करता है या सेट करता है जिसे बदला जा सकता है। |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | फ़िल्टर में FieldName, Test, और Value के साथ स्थापित मानदंड को प्राप्त करता है या सेट करता है, जो अन्य मानदंडों से संबंधित है। |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | फ़िल्टर के चयन मानदंड के रूप में कार्य करने वाले FieldName और Value के बीच किए गए तुलना प्रकार को प्राप्त करता है या सेट करता है। [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | FieldName द्वारा निर्दिष्ट फ़ील्ड के मान के साथ तुलना करने के लिए ऑब्जेक्ट मान प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | यह प्राप्त करता है कि FilterCriteria का दायाँ मान फ़ील्ड संदर्भ है या स्थिर मान नहीं। |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | उस फ़ील्ड को सेट करता है जिसका मान FieldName द्वारा निर्दिष्ट फ़ील्ड के मान के साथ तुलना किया जाएगा। |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | `FilterCriteria` क्लास के इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है। |

## उदाहरण

टास्क फ़िल्टर मानदंड को कैसे पढ़ें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// फ़िल्टर मानदंड को स्ट्रिंग के रूप में प्रिंट करें 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


