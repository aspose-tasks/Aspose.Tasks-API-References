---
title: "BuiltInProjectPropertyCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API 참조"
description: "BuiltInProjectPropertyCollection 속성. 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다(읽기 전용이 아니면 false)."
type: docs
weight: 60
url: /ko/net/aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/
---
## BuiltInProjectPropertyCollection.IsReadOnly property

이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false.

```csharp
public override bool IsReadOnly { get; }
```

## 예제

프로젝트 내장 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// 내장 속성 컬렉션을 반복합니다
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### 또 보기

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


