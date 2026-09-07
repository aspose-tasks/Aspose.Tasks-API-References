---
title: "BaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "BaselineCollection मेथड। इस संग्रह के लिए एक एनेमरेटर लौटाता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/baselinecollection/getenumerator/
---
## BaselineCollection.GetEnumerator method

इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

```csharp
public IEnumerator<Baseline> GetEnumerator()
```

### रिटर्न वैल्यू

इस संग्रह के लिए एक एनेमरेटर।

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


