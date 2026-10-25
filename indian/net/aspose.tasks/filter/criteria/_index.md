---
title: "Filter.Criteria"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Filter property. उन मानदंडों को प्राप्त या सेट करता है जिन्हें कार्यों या संसाधनों को MSP दृश्य में प्रदर्शित होने के लिए पूरा करना आवश्यक है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/filter/criteria/
---
## Filter.Criteria property

टास्क या रिसोर्सेज़ को MSP व्यू में प्रदर्शित होने के लिए आवश्यक मानदंड प्राप्त करता है या सेट करता है।

```csharp
public FilterCriteria Criteria { get; set; }
```

## उदाहरण

कार्य फ़िल्टर को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine(filter.Criteria.CriteriaRows.Count);
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine(criteria1.Test.ToString());
Console.WriteLine(criteria1.Field.ToString());
Console.WriteLine(criteria1.Values[0].ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine(criteria21.Test.ToString());
Console.WriteLine(criteria21.Field.ToString());
Console.WriteLine(criteria21.Values[0].ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine(criteria22.Test.ToString());
Console.WriteLine(criteria22.Field.ToString());
Console.WriteLine(criteria22.Values[0].ToString());
Console.WriteLine(filter.Criteria);
```

### संबंधित देखें

* class [FilterCriteria](../../filtercriteria/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


