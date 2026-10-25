---
title: "Asn.NotesText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. RTF 데이터에서 추출한 메모 평문 텍스트"
type: docs
weight: 350
url: /ko/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

RTF 데이터에서 추출한 메모의 일반 텍스트입니다.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## 예제

리소스 할당 메모를 가져오고/설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// 리소스 할당 생성
var assn = project.ResourceAssignments.Add(task, rsc);

// 리소스 할당 메모 설정
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


