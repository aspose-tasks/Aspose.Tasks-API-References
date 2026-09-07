---
title: "OutlineCodeDefinitionCollection.Item"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineCodeDefinitionCollection प्रॉपर्टी। निर्दिष्ट इंडेक्स पर तत्व को प्राप्त या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/outlinecodedefinitioncollection/item/
---
## OutlineCodeDefinitionCollection indexer

निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है।

```csharp
public OutlineCodeDefinition this[int index] { get; set; }
```

| पैरामीटर | विवरण |
| --- | --- |
| इंडेक्स | प्राप्त या सेट करने वाले तत्व का शून्य-आधारित अनुक्रमणिका। |

### रिटर्न वैल्यू

निर्दिष्ट अनुक्रमणिका पर तत्व।

## उदाहरण

Outline code definition संग्रहों के साथ कैसे काम किया जाए, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// एक कस्टम आउटलाइन कोड परिभाषा जोड़ें
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // स्थिति में outline code definition सम्मिलित करें
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// outline code definition का सूचकांक खोजें
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// आउटलाइन कोड परिभाषा को संपादित करें
project.OutlineCodes[index].Alias = "New Alias";

// ...
// आउटलाइन कोड परिभाषाओं के साथ काम करें
// ...

// आउटलाइन कोड परिभाषा को हटाएँ
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// सूचकांक द्वारा एक आउटलाइन कोड परिभाषा हटाएँ
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// आउटलाइन कोड परिभाषाओं को हटाएँ
otherProject.OutlineCodes.Clear();

// आउटलाइन कोड परिभाषाओं की प्रतिलिपि बनाएं
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// आउटलाइन कोड परिभाषाओं के साथ काम करें
// ...

// आउटलाइन कोड परिभाषाओं को एक-एक करके हटाएँ
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### संबंधित देखें

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


