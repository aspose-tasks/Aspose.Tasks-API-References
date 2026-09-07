---
title: "SplitPartCollection.Item"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SplitPartCollection प्रॉपर्टी। दिए गए इंडेक्स पर टास्क का स्प्लिट पार्ट प्राप्त करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

दिए गए इंडेक्स पर टास्क के स्प्लिट पार्ट को पुनः प्राप्त करता है।

```csharp
public SplitPart this[int index] { get; set; }
```

| पैरामीटर | विवरण |
| --- | --- |
| इंडेक्स | भाग का इंडेक्स। |

### रिटर्न वैल्यू

एक स्प्लिट पार्ट।

## टिप्पणियाँ

इंडेक्स शून्य-आधारित है। यदि इंडेक्स एरे की सीमाओं के बाहर है तो null लौटाता है।

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


