---
title: "ExtendedAttribute.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 메서드. 확장 속성의 짧은 문자열 표현을 반환합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

확장 속성의 짧은 문자열 표현을 반환합니다.

```csharp
public override string ToString()
```

### 반환 값

확장 속성의 문자열 표현입니다.

## 예제

확장 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// 작업에 대한 확장 속성을 읽습니다.
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // 확장 속성에 대한 일반 정보를 읽습니다.
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### 또 보기

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


