---
title: "क्लास EntityFieldAttribute"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute क्लास। एंटिटी प्रॉपर्टीज़ के लिए एक एट्रिब्यूट दर्शाती है।"
type: docs
weight: 70
url: /hi/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

इकाई गुणों के लिए एक विशेषता को दर्शाता है।

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## टिप्पणियाँ

केवल [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) और [`ResourceAssignment`](../../aspose.tasks/resourceassignment/) एंटिटी प्रॉपर्टीज़ के लिए उपयोग किया जाने वाला एट्रिब्यूट, और इसकी एन्उमरेशन को सरल बनाता है।

## उदाहरण

**EntityField** एट्रिब्यूट का उपयोग करके प्रॉपर्टीज़ को एन्उमरेट करने का तरीका:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### संबंधित देखें

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


