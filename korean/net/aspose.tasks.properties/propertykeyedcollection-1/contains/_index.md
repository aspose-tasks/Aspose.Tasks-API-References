---
title: "PropertyKeyedCollection1.Contains"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PropertyKeyedCollection 메서드. 지정된 이름을 가진 property가 PropertyCollection에 포함되어 있는지 확인합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks.properties/propertykeyedcollection-1/contains/
---
## PropertyKeyedCollection&lt;T&gt;.Contains method

지정된 이름을 가진 property가 [`PropertyCollection`](../../propertycollection-1/)에 포함되어 있는지 확인합니다.

```csharp
public bool Contains(string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | property의 이름 |

### 반환 값

지정된 이름을 가진 property가 [`PropertyCollection`](../../propertycollection-1/)에 포함되어 있으면 true; 그렇지 않으면 false.

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

* class [PropertyKeyedCollection&lt;T&gt;](../)
* namespace [Aspose.Tasks.Properties](../../propertykeyedcollection-1/)
* assembly [Aspose.Tasks](../../../)


