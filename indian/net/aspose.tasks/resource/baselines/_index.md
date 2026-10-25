---
title: "Resource.Baselines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी। इस ऑब्जेक्ट के लिए BaselineCollection का एक इंस्टेंस प्राप्त करता है। एक संसाधन के लिए बेसलाइन मान"
type: docs
weight: 160
url: /hi/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

इस ऑब्जेक्ट के लिए BaselineCollection का इंस्टेंस प्राप्त करता है। एक संसाधन के लिए बेसलाइन मान।

```csharp
public BaselineCollection Baselines { get; }
```

## उदाहरण

दिखाता है कि संसाधन की बेसलाइन कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### संबंधित देखें

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


