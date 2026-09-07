---
title: "क्लास OutlineCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OutlineCode क्लास। एक outline कोड के मान को दर्शाती है।"
type: docs
weight: 1150
url: /hi/net/aspose.tasks/outlinecode/
---
## OutlineCode class

एक रूपरेखा कोड का मान दर्शाता है।

```csharp
public class OutlineCode
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | `OutlineCode` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | निर्दिष्ट Outline Code और उसके एक मान का उपयोग करके `OutlineCode` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | प्रोजेक्ट Id कस्टम फ़ील्ड का संख्या मान प्राप्त करता है या सेट करता है। |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | वैल्यू लिस्ट में मान का GUID प्राप्त करता है या सेट करता है। ValueGuid वैल्यू लिस्ट में FieldGuid से मेल खाता है। |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | outline कोड संग्रह में परिभाषा से जुड़े वैल्यू लिस्ट में Id प्राप्त करता है या सेट करता है। |

## टिप्पणियाँ

दो डेटा आवश्यक हैं - FieldId द्वारा निर्दिष्ट outline कोड टेबल का पॉइंटर, और वह मान जो ValueId या ValueGuid पॉइंटर द्वारा वैल्यू लिस्ट में निर्दिष्ट किया गया है।

## उदाहरण

टास्क के outline कोड्स को पढ़ने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// outline कोड्स पढ़ें
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


