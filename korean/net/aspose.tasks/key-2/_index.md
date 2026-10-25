---
title: "구조체 KeyTK"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Key2TK 구조체. 지정된 유형의 클래스에 대한 속성 키를 나타냅니다. 이 클래스의 인스턴스는 컨테이너의 속성을 가져오거나 설정할 때 사용됩니다."
type: docs
weight: 930
url: /ko/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

지정된 유형의 클래스에 대한 속성 키를 나타냅니다. 이 클래스의 인스턴스는 컨테이너의 속성을 가져오거나 설정할 때 사용됩니다.

```csharp
public struct Key<T, K>
    where K : struct
```

| 매개변수 | 설명 |
| --- | --- |
| T | 속성 값의 유형입니다. |
| K | 속성 키의 유형입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | 속성의 키를 가져옵니다. |

## 예제

Prj.ActualsInSync 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


