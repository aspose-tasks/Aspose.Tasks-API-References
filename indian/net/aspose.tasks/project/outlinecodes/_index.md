---
title: "Project.OutlineCodes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। OutlineCodeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। प्रोजेक्ट से जुड़े आउटलाइन कोड परिभाषाओं का संग्रह"
type: docs
weight: 710
url: /hi/net/aspose.tasks/project/outlinecodes/
---
## Project.OutlineCodes property

OutlineCodeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। प्रोजेक्ट से जुड़े आउटलाइन कोड परिभाषाओं का संग्रह।

```csharp
public OutlineCodeDefinitionCollection OutlineCodes { get; }
```

## उदाहरण

आउटलाइन कोड पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

foreach (var ocd in project.OutlineCodes)
{
    Console.WriteLine("Alias = " + ocd.Alias);
    Console.WriteLine(ocd.AllLevelsRequired ? "It contains property: must have all levels" : "It does not contain property: must have all levels");
    Console.WriteLine(ocd.Enterprise ? "It is an enterprise custom outline code." : "It is not an enterprise custom outline code.");
    Console.WriteLine("Reference to another custom field for which this outline code definition is an alias is = " + ocd.EnterpriseOutlineCodeAlias);
    Console.WriteLine("Field Id = " + ocd.FieldId);
    Console.WriteLine("Field Name = " + ocd.FieldName);
    Console.WriteLine("Phonetic Alias = " + ocd.PhoneticAlias);
    Console.WriteLine("Guid = " + ocd.Guid);

    // आउटलाइन कोड मास्क प्रदर्शित करें
    foreach (var outlineMask in ocd.Masks)
    {
        Console.WriteLine("Level of a mask = " + outlineMask.Level);
        Console.WriteLine("Mask = " + outlineMask);
    }

    // आउटलाइन कोड मान प्रदर्शित करें
    foreach (var outlineMask1 in ocd.Values)
    {
        Console.WriteLine("Description of outline value = " + outlineMask1.Description);
        Console.WriteLine("Value Id = " + outlineMask1.ValueId);
        Console.WriteLine("Value = " + outlineMask1.Value);
        Console.WriteLine("Type = " + outlineMask1.Type);
    }
}
```

### संबंधित देखें

* class [OutlineCodeDefinitionCollection](../../outlinecodedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


