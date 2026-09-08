---
title: "Prj.Guid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 GUID"
type: docs
weight: 360
url: /ko/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

프로젝트의 GUID.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## 예제

Prj.Guid 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


