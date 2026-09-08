---
title: "Prj.Manager"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 관리자"
type: docs
weight: 450
url: /ko/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

프로젝트의 관리자.

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## 예제

Shows how to read/write Prj.Manager property.

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


