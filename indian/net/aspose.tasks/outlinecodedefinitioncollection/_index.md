---
title: "क्लास OutlineCodeDefinitionCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OutlineCodeDefinitionCollection क्लास। OutlineCodeDefinition ऑब्जेक्ट्स का संग्रह दर्शाता है।"
type: docs
weight: 1180
url: /hi/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

[`OutlineCodeDefinition`](../outlinecodedefinition/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | इस संग्रह में निर्दिष्ट आइटम का सूचकांक निर्धारित करता है। |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है। |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | निर्दिष्ट सूचकांक पर एक आइटम हटाता है। |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | इस OutlineCodeDefinitionCollection ऑब्जेक्ट को [`OutlineCodeDefinition`](../outlinecodedefinition/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


