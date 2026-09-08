---
title: "Prj.ProjectExternallyEdited"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트가 외부에서 편집되었는지 여부를 결정합니다."
type: docs
weight: 590
url: /ko/net/aspose.tasks/prj/projectexternallyedited/
---
## Prj.ProjectExternallyEdited field

프로젝트가 외부에서 편집되었는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> ProjectExternallyEdited;
```

## 예제

Prj.ProjectExternallyEdited 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.ProjectExternallyEdited, true);

Console.WriteLine("Project Externally Edited: " + project.Get(Prj.ProjectExternallyEdited));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


