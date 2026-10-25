---
title: "Prj.AdminProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트가 관리 프로젝트인지 여부를 결정합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

프로젝트가 관리 프로젝트인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## 예제

Prj.AdminProject 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


