---
title: "क्लास BaselineCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.BaselineCollection क्लास। Baseline ऑब्जेक्ट्स का संग्रह दर्शाती है।"
type: docs
weight: 120
url: /hi/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

[`Baseline`](../baseline/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class BaselineCollection : IList<Baseline>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | इस BaselineCollection ऑब्जेक्ट में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | इस संग्रह के लिए पैरेंट [`Resource`](../resource/) प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकती है। |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | इस संग्रह से बेसलाइन को हटाता है। |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | BaselineCollection ऑब्जेक्ट को [`Baseline`](../baseline/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

Baseline संग्रहों के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// Baseline जानकारी पढ़ें
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### संबंधित देखें

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


