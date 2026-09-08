---
title: "노트"
second_title: "Aspose.Tasks for .NET API 참조"
description: "리소스와 연결된 텍스트 메모."
type: docs
weight: 470
url: /ko/net/aspose.tasks/rsc/notes/
---
## Rsc.Notes field

리소스와 연결된 텍스트 메모.

```csharp
public static readonly Key<string, RscKey> Notes;
```

### 예제

Rsc.Notes 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Notes, "Resource Notes");

Console.WriteLine("Notes: " + resource.Get(Rsc.Notes));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
