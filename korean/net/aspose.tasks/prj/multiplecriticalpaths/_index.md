---
title: "Prj.MultipleCriticalPaths"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 여러 중요한 경로가 계산되는지 여부를 결정합니다."
type: docs
weight: 530
url: /ko/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

다중 임계 경로가 계산되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## 예제

Prj.MultipleCriticalPaths 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


