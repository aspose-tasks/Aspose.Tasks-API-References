---
title: "ExtendedAttributeDefinition.ValueList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition özelliği. ListValue ValueList'i alır"
type: docs
weight: 280
url: /tr/net/aspose.tasks/extendedattributedefinition/valuelist/
---
## ExtendedAttributeDefinition.ValueList property

List&lt;Value&gt; ValueList'i alır.

```csharp
public List<Value> ValueList { get; }
```

## Açıklamalar

Şema içindeki öğelerin özellikleri olarak genişletilmiş öznitelik değerleri belirtildiğinde, bu değerler ya doğrudan değerlerle ya da bu listedeki değerlerin referanslarıyla belirtilebilir. Uygulamalar, burada belirtilen sıralamaya göre listenin sıralanacağını varsayabilir. Şu anda MSP 2003/2007 Xml ve MSP 2003 mpp formatları için desteklenmektedir. Bu listeyi doğrudan değiştirmeyin. Bunun yerine ExtendedAttributeDefinition.AddLookupValue/RemoveLookupValue yöntemlerini kullanın.

## Örnekler

Genişletilmiş öznitelik tanımının ortak bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// genişletilmiş öznitelik tanımı bilgilerini oku
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

### Ayrıca Bakınız

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


