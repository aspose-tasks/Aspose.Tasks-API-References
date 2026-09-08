---
title: "열거형 CustomPropertyType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Properties.CustomPropertyType 열거형. 사용자 정의 속성 유형 열거형을 나타냅니다."
type: docs
weight: 1560
url: /ko/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

사용자 정의 속성 유형 열거형을 나타냅니다.

```csharp
public enum CustomPropertyType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | 속성에 유형이 없습니다. |
| String | `1` | 속성은 문자열 값입니다. |
| DateTime | `2` | 속성은 날짜 및 시간 값입니다. |
| Number | `3` | 속성은 정수 값입니다. |
| Boolean | `4` | 속성은 부울 값입니다. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


