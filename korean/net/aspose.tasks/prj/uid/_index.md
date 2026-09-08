---
title: "Prj.Uid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 고유 ID입니다"
type: docs
weight: 760
url: /ko/net/aspose.tasks/prj/uid/
---
## Prj.Uid field

프로젝트의 고유 Id.

```csharp
public static readonly Key<string, PrjKey> Uid;
```

## 예제

Prj.Uid 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Uid, "1234");

Console.WriteLine("Uid: " + project.Get(Prj.Uid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


