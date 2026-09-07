---
title: "एनम FilterOperation"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.FilterOperation एनम। यह निर्दिष्ट करता है कि FieldName, FilterComparisonType और Value के साथ स्थापित मानदंड फ़िल्टर में अन्य मानदंडों से कैसे संबंधित है।"
type: docs
weight: 640
url: /hi/net/aspose.tasks/filteroperation/
---
## FilterOperation enumeration

फ़ील्डनाम, FilterComparisonType, और वैल्यू के साथ स्थापित मानदंड फ़िल्टर में अन्य मानदंडों से कैसे संबंधित है, यह निर्दिष्ट करता है।

```csharp
public enum FilterOperation
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `0` | अपरिभाषित। |
| And | `1` | AND ऑपरेटर। |
| Or | `2` | OR ऑपरेटर। |

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


