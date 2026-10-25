---
title: "노트"
second_title: "Aspose.Tasks for .NET API 참조"
description: "과제와 연결된 텍스트 메모."
type: docs
weight: 350
url: /ko/net/aspose.tasks/asn/notes/
---
## Asn.Notes field

과제와 연결된 텍스트 메모.

```csharp
public static readonly Key<string, AsnKey> Notes;
```

### 예제

리소스 할당 메모를 가져오고/설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// 리소스 할당 생성
var assn = project.ResourceAssignments.Add(task, rsc);

// 리소스 할당 메모 설정
assn.Set(Asn.Notes, "Newly added assignment");

Console.WriteLine("Notes: " + assn.Get(Asn.Notes));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
