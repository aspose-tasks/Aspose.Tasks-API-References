---
title: "ExtendedAttributeDefinition.FieldId"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition प्रॉपर्टी। कस्टम फ़ील्ड के प्रोजेक्ट ID से संबंधित प्राप्त करता है या सेट करता है। FieldId प्रॉपर्टी निर्दिष्ट करने के लिए ExtendedAttributeTask क्लास की एक स्थिरांक की स्ट्रिंग प्रतिनिधित्व का उपयोग करें"
type: docs
weight: 130
url: /hi/net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

कस्टम फ़ील्ड के प्रोजेक्ट ID से संबंधित प्राप्त करता है या सेट करता है। FieldId प्रॉपर्टी निर्दिष्ट करने के लिए [`ExtendedAttributeTask`](../../extendedattributetask/) क्लास की एक स्थिरांक की स्ट्रिंग प्रतिनिधित्व का उपयोग करें।

```csharp
public string FieldId { get; set; }
```

## टिप्पणियाँ

`FieldId` प्रॉपर्टी सेट करने का पसंदीदा तरीका है कि [`ExtendedAttributeDefinition`](../) को एक समर्पित फ़ैक्टरी मेथड जैसे [`CreateTaskDefinition`](../createtaskdefinition/) या [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/) का उपयोग करके बनाया जाए।

## उदाहरण

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

विस्तारित एट्रिब्यूट परिभाषा की सामान्य जानकारी को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// विस्तारित एट्रिब्यूट परिभाषा की जानकारी पढ़ें
foreach (var definition in project.ExtendedAttributes)
{
    Console.WriteLine("Guid:" + definition.Guid);
    Console.WriteLine("Secondary Guid:" + definition.SecondaryGuid);
    Console.WriteLine("Secondary Pid:" + definition.SecondaryPid);
    Console.WriteLine("Alias:" + definition.Alias);
    Console.WriteLine("Phonetics Alias:" + definition.PhoneticsAlias);
    Console.WriteLine("Field Id:" + definition.FieldId);
    Console.WriteLine("Project Name:" + definition.ParentProject.Get(Prj.Name));

    Console.WriteLine("Append New Values:" + definition.AppendNewValues);
    Console.WriteLine("Auto RollDown:" + definition.AutoRollDown);
    Console.WriteLine("Calculation Type:" + definition.CalculationType);
    Console.WriteLine("Field Name" + definition.FieldName);
    Console.WriteLine("Is User Defined Custom Field:" + definition.UserDef);
    Console.WriteLine("Rollup Type:" + definition.RollupType);

    if (definition.CalculationType == CalculationType.Lookup)
    {
        Console.WriteLine("  Next properties are used only for lookups:");
        Console.WriteLine("  Default Guid:" + definition.DefaultGuid);
        Console.WriteLine("  Element Type:" + definition.ElementType);
        Console.WriteLine("  Lookup Uid:" + definition.LookupUid);
        Console.WriteLine("  Restrict Values:" + definition.RestrictValues);
        Console.WriteLine("  Max Multi Values:" + definition.MaxMultiValues);
        Console.WriteLine("  Valuelist Sort Order:" + definition.ValuelistSortOrder);
        Console.WriteLine("  Default Value:" + definition.Default);
        Console.WriteLine("  Print values from value list:");
        foreach (var value in definition.ValueList)
        {
            Console.WriteLine("    Description: " + value.Description);
            Console.WriteLine("    Value: " + value.Val);
        }
    }

    Console.WriteLine();
}
```

### संबंधित देखें

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


