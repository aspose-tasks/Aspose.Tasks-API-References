---
title: "क्लास SplitPartCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.SplitPartCollection क्लास। यह कलेक्शन टास्क के भागों को दर्शाता है।"
type: docs
weight: 2300
url: /hi/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

एक कार्य के भागों को दर्शाने वाला संग्रह।

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | कलेक्शन में भागों की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | दिए गए इंडेक्स पर टास्क के स्प्लिट पार्ट को पुनः प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | कलेक्शन से सभी भागों को नई एरे में कॉपी करता है। |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


