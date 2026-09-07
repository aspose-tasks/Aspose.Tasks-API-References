---
title: "एनम FilterComparisonType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.FilterComparisonType एनम। वह तुलना प्रकार जो FieldName और Value के बीच किया जाता है और फ़िल्टर या ग्राफ़िकल इंडिकेटर के लिए चयन मानदंड के रूप में कार्य करता है।"
type: docs
weight: 620
url: /hi/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

फ़ील्डनाम और वैल्यू के बीच किए गए तुलना के प्रकार को निर्दिष्ट करता है जो फ़िल्टर या ग्राफ़िकल संकेतक के लिए चयन मानदंड के रूप में कार्य करता है।

```csharp
public enum FilterComparisonType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Equals | `6` | Field का मान Value के बराबर है। |
| DoesNotEqual | `7` | Field का मान Value के बराबर नहीं है। |
| IsGreaterThan | `2` | Field का मान Value से बड़ा है। |
| IsGreaterThanOrEqualTo | `4` | Field का मान Value से बड़ा या उसके बराबर है। |
| IsLessThan | `3` | Field का मान Value से छोटा है। |
| IsLessThanOrEqualTo | `5` | Field का मान Value से छोटा या उसके बराबर है। |
| IsWithin | `1` | Field का मान Value के भीतर है। |
| IsNotWithin | `9` | Field का मान Value के भीतर नहीं है। |
| Contains | `8` | Field का मान Value को शामिल करता है। |
| DoesNotContain | `10` | Field का मान Value को शामिल नहीं करता है। |
| ContainsExactly | `11` | Field का मान बिल्कुल Value को शामिल करता है। |
| IsOneOf | `12` | Field का मान निर्दिष्ट मानों में से किसी एक के बराबर है। AutoFilters में उपयोग किया जाता है। |
| Undefined | `0` | अपरिभाषित मान। |
| IsAnyValue | `255` | 'Is any value' शर्त। ग्राफ़िकल इंडिकेटर्स पर लागू होती है। |

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


