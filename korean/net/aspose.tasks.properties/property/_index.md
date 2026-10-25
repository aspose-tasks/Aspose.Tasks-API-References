---
title: "클래스 Property"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Properties.Property 클래스. 속성의 기본 클래스를 나타냅니다"
type: docs
weight: 1580
url: /ko/net/aspose.tasks.properties/property/
---
## Property class

속성의 기본 클래스를 나타냅니다.

```csharp
public abstract class Property
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | 속성의 이름을 가져옵니다. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | 속성의 값을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | 속성 값을 문자열로 반환합니다. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


