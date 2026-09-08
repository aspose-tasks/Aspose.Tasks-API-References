---
title: "ExtendedAttributeDefinition.ValueList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 속성. ListValue ValueList를 가져옵니다"
type: docs
weight: 280
url: /ko/net/aspose.tasks/extendedattributedefinition/valuelist/
---
## ExtendedAttributeDefinition.ValueList property

List&lt;Value&gt; ValueList를 가져옵니다.

```csharp
public List<Value> ValueList { get; }
```

## 비고

스키마의 요소 속성으로 확장 속성 값을 지정할 때, 해당 값은 직접 값으로 지정하거나 이 목록에 포함된 값에 대한 참조로 지정할 수 있습니다. 응용 프로그램은 여기에서 지정된 순서를 통해 목록의 순서를 가정할 수 있습니다. 현재 MSP 2003/2007 Xml 및 MSP 2003 mpp 형식에서 지원됩니다. 이 목록을 직접 변경하지 마십시오. 대신 ExtendedAttributeDefinition.AddLookupValue/RemoveLookupValue 메서드를 사용하십시오.

## 예제

확장 속성 정의의 일반 정보를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// 확장 속성 정의 정보를 읽습니다
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

### 또 보기

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


