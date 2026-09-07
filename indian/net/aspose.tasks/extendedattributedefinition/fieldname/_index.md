---
title: "ExtendedAttributeDefinition.FieldName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition प्रॉपर्टी। एक कस्टम फ़ील्ड का नाम प्राप्त करता है"
type: docs
weight: 140
url: /hi/net/aspose.tasks/extendedattributedefinition/fieldname/
---
## ExtendedAttributeDefinition.FieldName property

कस्टम फ़ील्ड का नाम प्राप्त करता है।

```csharp
public string FieldName { get; }
```

## टिप्पणियाँ

इसे सीधे सेट नहीं किया जाना चाहिए, बल्कि ExtendedAttributeDefinition को स्ट्रॉन्गली टाइप्ड स्टैटिक फ़ैक्टरी मेथड्स जैसे Create*Definition() का उपयोग करके बनाना चाहिए।

## उदाहरण

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


