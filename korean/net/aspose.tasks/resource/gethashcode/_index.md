---
title: "Resource.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 메서드. Resource 클래스 인스턴스에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 840
url: /ko/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

[`Resource`](../) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

리소스의 해시 코드를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// 리소스의 해시 코드는 리소스 UID와 같습니다.
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### 또 보기

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


