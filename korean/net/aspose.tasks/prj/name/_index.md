---
title: "Prj.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 이름"
type: docs
weight: 540
url: /ko/net/aspose.tasks/prj/name/
---
## Prj.Name field

프로젝트 이름.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## 예제

프로젝트 이름을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


