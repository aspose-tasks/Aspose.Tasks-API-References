---
title: "클래스 CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Properties.CustomProjectPropertyCollection 클래스. 사용자 정의 프로젝트 속성 컬렉션을 나타냅니다."
type: docs
weight: 1550
url: /ko/net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

사용자 정의 프로젝트 속성 컬렉션을 나타냅니다.

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | `CustomProjectPropertyCollection` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | 새 사용자 정의 속성을 생성합니다. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | 새 사용자 정의 속성을 생성합니다. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | 새 사용자 정의 속성을 생성합니다. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | 새 사용자 정의 속성을 생성합니다. |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | PropertyCollection을 비웁니다. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | 컬렉션에서 지정된 이름을 가진 속성을 제거합니다. |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


