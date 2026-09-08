---
title: "Project.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. ExtendedAttributeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 확장 속성 사용자 정의 필드 정의 컬렉션입니다."
type: docs
weight: 410
url: /ko/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

ExtendedAttributeDefinitionCollection 객체를 가져옵니다. 프로젝트와 연결된 확장 속성(사용자 정의 필드) 정의 컬렉션입니다.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## 예제

확장 속성을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// 프로젝트에 사용자 정의 필드가 없으면 생성합니다.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// 정의에서 확장 속성을 생성합니다.
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// 작업에 확장 속성을 추가합니다.
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


