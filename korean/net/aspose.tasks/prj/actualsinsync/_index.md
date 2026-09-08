---
title: "Prj.ActualsInSync"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 모든 실제 작업이 프로젝트와 동기화되었는지 여부를 결정합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

모든 실제 작업이 프로젝트와 동기화되었는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## 예제

Prj.ActualsInSync 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


