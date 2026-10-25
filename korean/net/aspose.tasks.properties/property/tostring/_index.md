---
title: "Property.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Property method. 속성 값을 문자열로 반환합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks.properties/property/tostring/
---
## Property.ToString method

속성 값을 문자열로 반환합니다.

```csharp
public override string ToString()
```

### 반환 값

문자열 값.

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

* class [Property](../)
* namespace [Aspose.Tasks.Properties](../../property/)
* assembly [Aspose.Tasks](../../../)


