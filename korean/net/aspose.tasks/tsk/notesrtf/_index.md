---
title: "Tsk.NotesRTF"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. RTF 형식의 텍스트 메모. MPP 형식에만 지원됩니다"
type: docs
weight: 820
url: /ko/net/aspose.tasks/tsk/notesrtf/
---
## Tsk.NotesRTF field

RTF 형식의 텍스트 메모입니다. MPP 형식에서만 지원됩니다.

```csharp
public static readonly Key<string, TaskKey> NotesRTF;
```

## 예제

Tsk.NotesRTF 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

            var task = project.RootTask.Children.Add("Task");

            const string rtf = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            task.Set(Tsk.NotesRTF, rtf);

            Console.WriteLine("Notes RTF: " + task.Get(Tsk.NotesRTF));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


