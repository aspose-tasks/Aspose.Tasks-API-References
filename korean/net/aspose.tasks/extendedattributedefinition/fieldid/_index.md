---
title: "ExtendedAttributeDefinition.FieldId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 속성. 사용자 정의 필드의 프로젝트 ID에 해당합니다. FieldId 속성을 지정하려면 ExtendedAttributeTask 클래스의 상수 문자열 표현을 사용하십시오."
type: docs
weight: 130
url: /ko/net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

사용자 정의 필드의 프로젝트 ID에 해당합니다. `FieldId` 속성을 지정하려면 [`ExtendedAttributeTask`](../../extendedattributetask/) 클래스의 상수 문자열 표현을 사용하십시오.

```csharp
public string FieldId { get; set; }
```

## 비고

`FieldId` 속성을 설정하는 권장 방법은 [`CreateTaskDefinition`](../createtaskdefinition/) 또는 [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/)와 같은 전용 팩터리 메서드 중 하나를 사용하여 [`ExtendedAttributeDefinition`](../)을 만드는 것입니다.

## 예제

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

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


