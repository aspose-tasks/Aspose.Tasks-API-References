---
title: "Rsc.NotesText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. RTF 데이터에서 추출한 메모 순수 텍스트"
type: docs
weight: 480
url: /ko/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

RTF 데이터에서 추출한 메모의 일반 텍스트입니다.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## 예제

Rsc.NotesText 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


