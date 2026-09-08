---
title: "ExtendedAttributeDefinitionCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinitionCollection 메서드. 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/extendedattributedefinitioncollection/remove/
---
## ExtendedAttributeDefinitionCollection.Remove method

이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다.

```csharp
public bool Remove(ExtendedAttributeDefinition item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | ExtendedAttributeDefinition | 제거할 지정된 객체. |

### 반환 값

지정된 객체가 이 컬렉션에서 성공적으로 제거되면 true; 그렇지 않으면 false.

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

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


