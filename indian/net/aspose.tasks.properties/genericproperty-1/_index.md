---
title: "स्ट्रक्ट GenericPropertyTKey"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Properties.GenericProperty1TKey स्ट्रक्ट। एक कंटेनर प्रॉपर्टी को दर्शाता है"
type: docs
weight: 1570
url: /hi/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

कंटेनर प्रॉपर्टी का प्रतिनिधित्व करता है।

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| पैरामीटर | विवरण |
| --- | --- |
| TKey | प्रॉपर्टी मान का प्रकार। |

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | `GenericProperty` स्ट्रक्ट का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | प्रॉपर्टी का नाम प्राप्त करता है। |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | प्रॉपर्टी का मान प्राप्त करता है। |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


