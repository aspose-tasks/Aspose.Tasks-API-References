---
title: "ExtendedAttributeDefinition.ValueList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition प्रॉपर्टी। ListValue ValueList प्राप्त करता है"
type: docs
weight: 280
url: /hi/net/aspose.tasks/extendedattributedefinition/valuelist/
---
## ExtendedAttributeDefinition.ValueList property

List&lt;Value&gt; ValueList प्राप्त करता है।

```csharp
public List<Value> ValueList { get; }
```

## टिप्पणियाँ

जब विस्तारित विशेषताओं के मान स्कीमा में तत्वों की प्रॉपर्टी के रूप में निर्दिष्ट किए जाते हैं, तो उन्हें मानों द्वारा या इस सूची में मौजूद मानों के संदर्भ द्वारा निर्दिष्ट किया जा सकता है। एप्लिकेशन यहाँ निर्दिष्ट क्रम के अनुसार सूची के क्रम को मान सकते हैं। वर्तमान में MSP 2003/2007 Xml और MSP 2003 mpp फ़ॉर्मेट के लिए समर्थित है। इस सूची को सीधे न बदलें। इसके बजाय ExtendedAttributeDefinition.AddLookupValue/RemoveLookupValue मेथड्स का उपयोग करें।

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

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


