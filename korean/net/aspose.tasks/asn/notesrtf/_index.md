---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. RTF 형식의 텍스트 메모. MPP 형식에서만 지원됩니다."
type: docs
weight: 340
url: /ko/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

RTF 형식의 텍스트 메모입니다. MPP 형식에서만 지원됩니다.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
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


