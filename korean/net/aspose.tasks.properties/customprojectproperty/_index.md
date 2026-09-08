---
title: "클래스 CustomProjectProperty"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Properties.CustomProjectProperty 클래스. 사용자 정의 속성을 나타냅니다."
type: docs
weight: 1540
url: /ko/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

사용자 정의 속성을 나타냅니다.

```csharp
public sealed class CustomProjectProperty : Property
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | 속성의 이름을 가져옵니다. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | 속성의 유형을 가져옵니다. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | 속성의 값을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | 속성 값을 문자열로 반환합니다. |

## 예제

맞춤형 프로젝트 속성 컬렉션 작업 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// 새 맞춤형 속성을 추가해 봅시다
// 컬렉션은 Boolean, DateTime, Double, String 유형을 지원합니다.
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// 맞춤형 속성은 타입이 지정된 컬렉션을 통해 사용할 수 있습니다.
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// 맞춤형 속성 값을 가져옵니다.
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// 맞춤형 속성 이름을 반복합니다.
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// 문자열 키로 값을 삭제할 수 있습니다.
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// 또는 컬렉션을 완전히 비울 수 있습니다
project.CustomProps.Clear();
```

### 또 보기

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


