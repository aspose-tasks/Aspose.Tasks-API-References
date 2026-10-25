---
title: "SplitPartCollection.ToArray"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SplitPartCollection मेथड। संग्रह से सभी भागों को नई एरे में कॉपी करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

कलेक्शन से सभी भागों को नई एरे में कॉपी करता है।

```csharp
public SplitPart[] ToArray()
```

### रिटर्न वैल्यू

[`SplitPart`](../../splitpart/) ऑब्जेक्ट्स की एक एरे।

## उदाहरण

स्प्लिट पार्ट कलेक्शन्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// स्प्लिट पार्ट्स पर इटरेट करें
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// इंडेक्स द्वारा भाग प्राप्त करें
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// टास्क के पहले स्प्लिट पार्ट के साथ कुछ काम करें
```

### संबंधित देखें

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


