---
title: "Project.BuiltInProps"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 프로젝트 내장 속성 컬렉션을 가져옵니다"
type: docs
weight: 100
url: /ko/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

프로젝트의 내장 속성 컬렉션을 가져옵니다.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
```

## 예제

프로젝트 메타 속성을 읽는 방법을 보여줍니다 (구식 API).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// 맞춤형 속성은 타입이 지정된 컬렉션을 통해 사용할 수 있습니다.
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// 내장 속성을 직접 사용할 수 있습니다.
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// 또는 내장 속성 컬렉션의 항목으로 사용할 수 있습니다.
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### 또 보기

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


