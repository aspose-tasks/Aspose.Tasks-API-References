---
title: "클래스 OutlineCodeDefinitionCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineCodeDefinitionCollection 클래스. OutlineCodeDefinition 객체의 컬렉션을 나타냅니다."
type: docs
weight: 1180
url: /ko/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

[`OutlineCodeDefinition`](../outlinecodedefinition/) 객체의 컬렉션을 나타냅니다.

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | 이 OutlineCodeDefinitionCollection 객체를 [`OutlineCodeDefinition`](../outlinecodedefinition/) 객체 목록으로 변환합니다. |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


