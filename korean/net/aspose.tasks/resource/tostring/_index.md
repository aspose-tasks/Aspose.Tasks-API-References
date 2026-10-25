---
title: "Resource.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 메서드. Resource 클래스 인스턴스의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 명시되지 않았으며 변경될 수 있습니다."
type: docs
weight: 870
url: /ko/net/aspose.tasks/resource/tostring/
---
## Resource.ToString method

[`Resource`](../) 클래스 인스턴스의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 명시되지 않았으며 변경될 수 있습니다.

```csharp
public override string ToString()
```

### 반환 값

리소스 객체를 나타내는 짧은 문자열.

## 예제

리소스 ToString 메서드 사용 방법을 보여줍니다.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// 리소스 일반 정보를 출력합니다
Console.WriteLine(resource.ToString());
```

### 또 보기

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


