---
title: "Prj.Autolink"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 삽입되거나 이동된 작업이 자동으로 연결되는지 여부를 결정합니다"
type: docs
weight: 70
url: /ko/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

삽입되거나 이동된 작업이 자동으로 연결되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## 예제

Prj.Autolink 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


