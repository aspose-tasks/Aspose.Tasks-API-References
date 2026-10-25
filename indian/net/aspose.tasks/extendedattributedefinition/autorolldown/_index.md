---
title: "ExtendedAttributeDefinition.AutoRollDown"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त या सेट करता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं"
type: docs
weight: 70
url: /hi/net/aspose.tasks/extendedattributedefinition/autorolldown/
---
## ExtendedAttributeDefinition.AutoRollDown property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं।

```csharp
public bool AutoRollDown { get; set; }
```

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


