---
title: "클래스 PropertyKeyedCollectionT"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Properties.PropertyKeyedCollection1T 클래스. 속성 컬렉션의 기본 클래스"
type: docs
weight: 1600
url: /ko/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

속성 컬렉션의 기본 클래스를 나타냅니다.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| 매개변수 | 설명 |
| --- | --- |
| T | 속성의 유형. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | 컬렉션에 포함된 속성 수를 가져옵니다. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | 지정된 키와 연결된 Property를 가져옵니다. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | 모든 속성 이름의 컬렉션을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | 새 사용자 정의 속성을 생성합니다. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | 지정된 이름을 가진 속성이 [`PropertyCollection`](../propertycollection-1/)에 포함되어 있는지 확인합니다. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


