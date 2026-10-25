---
title: "ExtendedAttributeDefinition.AppendNewValues"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 속성. 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 가져오거나 설정합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/extendedattributedefinition/appendnewvalues/
---
## ExtendedAttributeDefinition.AppendNewValues property

프로젝트에 추가된 새 값이 목록에 자동으로 추가되는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool AppendNewValues { get; set; }
```

## 비고

현재 MSP 2003/2007 Xml 및 MSP 2003 mpp 형식을 지원합니다.

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

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


