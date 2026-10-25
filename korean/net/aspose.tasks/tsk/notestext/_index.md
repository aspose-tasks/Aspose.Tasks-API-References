---
title: "Tsk.NotesText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. RTF 데이터에서 추출한 메모의 일반 텍스트입니다."
type: docs
weight: 830
url: /ko/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

RTF 데이터에서 추출한 메모의 일반 텍스트입니다.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## 예제

Tsk.NotesText 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


