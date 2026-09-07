---
title: "Project.BuiltInProps"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। प्रोजेक्ट की बिल्ट‑इन प्रॉपर्टीज़ संग्रह प्राप्त करता है"
type: docs
weight: 100
url: /hi/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

प्रोजेक्ट की बिल्ट-इन प्रॉपर्टीज़ कलेक्शन प्राप्त करता है।

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट मेटा प्रॉपर्टीज़ (पुरानी API) को कैसे पढ़ा जाए।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// कस्टम प्रॉपर्टीज़ टाइप्ड संग्रह के माध्यम से उपलब्ध हैं
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// बिल्ट-इन प्रॉपर्टीज़ सीधे उपलब्ध हैं
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// या बिल्ट-इन प्रॉपर्टी संग्रह के एक आइटम के रूप में
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### संबंधित देखें

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


