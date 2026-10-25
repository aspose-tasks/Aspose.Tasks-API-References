---
title: "Prj.Template"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트 템플릿"
type: docs
weight: 720
url: /ko/net/aspose.tasks/prj/template/
---
## Prj.Template field

프로젝트 템플릿.

```csharp
public static readonly Key<string, PrjKey> Template;
```

## 예제

Prj.Template 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Template, "Custom Template");

Console.WriteLine("Template: " + project.Get(Prj.Template));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


