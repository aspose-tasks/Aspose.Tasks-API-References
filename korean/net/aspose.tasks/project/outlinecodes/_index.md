---
title: "Project.OutlineCodes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. OutlineCodeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 개요 코드 정의 컬렉션입니다."
type: docs
weight: 710
url: /ko/net/aspose.tasks/project/outlinecodes/
---
## Project.OutlineCodes property

OutlineCodeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 개요 코드 정의의 컬렉션입니다.

```csharp
public OutlineCodeDefinitionCollection OutlineCodes { get; }
```

## 예제

개요 코드를 읽는 방법을 보여줍니다.

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

    // 개요 코드 마스크를 표시합니다.
    foreach (var outlineMask in ocd.Masks)
    {
        Console.WriteLine("Level of a mask = " + outlineMask.Level);
        Console.WriteLine("Mask = " + outlineMask);
    }

    // 개요 코드 값을 표시합니다.
    foreach (var outlineMask1 in ocd.Values)
    {
        Console.WriteLine("Description of outline value = " + outlineMask1.Description);
        Console.WriteLine("Value Id = " + outlineMask1.ValueId);
        Console.WriteLine("Value = " + outlineMask1.Value);
        Console.WriteLine("Type = " + outlineMask1.Type);
    }
}
```

### 또 보기

* class [OutlineCodeDefinitionCollection](../../outlinecodedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


