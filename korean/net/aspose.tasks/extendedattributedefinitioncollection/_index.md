---
title: "클래스 ExtendedAttributeDefinitionCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ExtendedAttributeDefinitionCollection 클래스. ExtendedAttributeDefinition 객체의 컬렉션을 나타냅니다."
type: docs
weight: 550
url: /ko/net/aspose.tasks/extendedattributedefinitioncollection/
---
## ExtendedAttributeDefinitionCollection class

[`ExtendedAttributeDefinition`](../extendedattributedefinition/) 객체의 컬렉션을 나타냅니다.

```csharp
public class ExtendedAttributeDefinitionCollection : IList<ExtendedAttributeDefinition>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributedefinitioncollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/extendedattributedefinitioncollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [Item](../../aspose.tasks/extendedattributedefinitioncollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |
| [ParentProject](../../aspose.tasks/extendedattributedefinitioncollection/parentproject/) { get; } | `ExtendedAttributeDefinitionCollection` 인스턴스의 상위 프로젝트를 가져옵니다. 이 컬렉션의 상위 프로젝트를 반환합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributedefinitioncollection/add/)(ExtendedAttributeDefinition) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/extendedattributedefinitioncollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/extendedattributedefinitioncollection/contains/)(ExtendedAttributeDefinition) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/extendedattributedefinitioncollection/copyto/)(ExtendedAttributeDefinition[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetById](../../aspose.tasks/extendedattributedefinitioncollection/getbyid/)(int) | ID로 확장 속성 정의를 반환합니다. |
| [GetEnumerator](../../aspose.tasks/extendedattributedefinitioncollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/extendedattributedefinitioncollection/indexof/)(ExtendedAttributeDefinition) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/extendedattributedefinitioncollection/insert/)(int, ExtendedAttributeDefinition) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/extendedattributedefinitioncollection/remove/)(ExtendedAttributeDefinition) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/extendedattributedefinitioncollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |
| [ToList](../../aspose.tasks/extendedattributedefinitioncollection/tolist/)() | 이 ExtendedAttributeDefinitionCollection 객체를 [`ExtendedAttributeDefinition`](../extendedattributedefinition/) 클래스의 인스턴스를 포함하는 리스트로 변환합니다. |

## 예제

확장 속성 정의 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // 확장 속성 정의를 지웁니다
        project.ExtendedAttributes.Clear();
    }
}

// 작업에 대한 확장 속성 정의를 생성합니다
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// 확장 속성 정의와 작업합니다...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// 확장 속성 정의와 작업합니다...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// 확장 속성 정의와 작업합니다...

// 인덱스로 확장 속성을 제거합니다
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// 컬렉션 인덱스 접근을 사용합니다
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// 속성을 다른 프로젝트에 복사합니다
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// 모든 확장 속성 정의를 제거합니다
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### 또 보기

* class [ExtendedAttributeDefinition](../extendedattributedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


