---
title: "CustomProjectPropertyCollection.CustomProjectPropertyCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CustomProjectPropertyCollection कंस्ट्रक्टर। CustomProjectPropertyCollection क्लास का एक नया उदाहरण इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.properties/customprojectpropertycollection/customprojectpropertycollection/
---
## CustomProjectPropertyCollection constructor

[`CustomProjectPropertyCollection`](../) क्लास का एक नया उदाहरण इनिशियलाइज़ करता है।

```csharp
public CustomProjectPropertyCollection()
```

## उदाहरण

दिखाता है कि कस्टम प्रोजेक्ट प्रॉपर्टी संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// आइए नई कस्टम प्रॉपर्टीज़ जोड़ें
// संग्रह Boolean, DateTime, Double, String प्रकारों का समर्थन करता है
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// कस्टम प्रॉपर्टीज़ टाइप्ड संग्रह के माध्यम से उपलब्ध हैं
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// कस्टम प्रॉपर्टी मान प्राप्त करें
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// कस्टम प्रॉपर्टीज़ के नामों पर इटरेट करें
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// एक स्ट्रिंग कुंजी द्वारा मान को हटाया जा सकता है
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// या कोई संग्रह को पूरी तरह से साफ़ कर सकता है
project.CustomProps.Clear();
```

### संबंधित देखें

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


