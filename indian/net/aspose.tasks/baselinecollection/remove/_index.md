---
title: "BaselineCollection.Remove"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "BaselineCollection मेथड। इस संग्रह से बेसलाइन को हटाता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

इस संग्रह से बेसलाइन को हटाता है।

```csharp
public bool Remove(Baseline item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आइटम | Baseline | हटाने के लिए आइटम। |

### रिटर्न वैल्यू

यदि [`Baseline`](../../baseline/) इंस्टेंस सफलतापूर्वक हटाया गया है तो true; अन्यथा false।

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


