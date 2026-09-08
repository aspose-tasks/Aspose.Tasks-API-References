---
title: "OutlineCodeDefinitionCollection.Contains"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineCodeDefinitionCollection 메서드. 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/outlinecodedefinitioncollection/contains/
---
## OutlineCodeDefinitionCollection.Contains method

지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

```csharp
public bool Contains(OutlineCodeDefinition item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | OutlineCodeDefinition | 찾을 지정된 항목. |

### 반환 값

지정된 항목이 이 컬렉션에 있으면 true; 그렇지 않으면 false.

## 예제

outline code definition 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// 사용자 지정 아웃라인 코드 정의를 추가합니다.
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // 지정 위치에 outline code definition을 삽입합니다.
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// outline code definition의 인덱스를 찾습니다.
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// 개요 코드 정의를 편집합니다
project.OutlineCodes[index].Alias = "New Alias";

// ...
// 개요 코드 정의를 다룹니다
// ...

// 개요 코드 정의를 제거합니다
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// 인덱스로 개요 코드 정의를 제거합니다
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// 개요 코드 정의들을 제거합니다
otherProject.OutlineCodes.Clear();

// 개요 코드 정의를 복사합니다
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// 개요 코드 정의를 다룹니다
// ...

// 개요 코드 정의를 하나씩 제거합니다
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### 또 보기

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


